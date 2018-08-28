---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 0
info:
  title: AWS Auto Scaling API Enter Standby
  version: 1.0.0
  description: Moves the specified instances into Standby mode.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EnterStandby:
    get:
      summary: Enter Standby
      description: Moves the specified instances into Standby mode.
      operationId: enterStandby
      x-api-path-slug: actionenterstandby-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group
        type: string
      - in: query
        name: InstanceIds.member.N
        description: One or more instances to move into Standby mode
        type: string
      - in: query
        name: ShouldDecrementDesiredCapacity
        description: Specifies whether the instances moved to Standby mode count as
          part of the Auto Scaling groups desired capacity
        type: string
      responses:
        200:
          description: OK
      tags:
      - Stand By
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---