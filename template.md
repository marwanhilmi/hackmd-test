# v2.1.17
**Launch Window** 11/24 2pm PST
**Branch** https://github.com/88dots/project-aperion/compare/v2.3.15
**Gamelift Queue** https://us-west-2.console.aws.amazon.com/gamelift/home?region=us-west-2#/r/game-session-queues/prod-stable-2-1-17

- [x] [**API**] Deploy prod-stable API https://buildkite.com/cpg/godfall/builds/2453
- [x] [**TEST**] Validate ap-iot crash is resolved
- [x] [**API**] Disable prod-beta/prod-smoke API
- [x] [**GAMELIFT**] Scale Server Fleets to production capacity
- [x] [**GAMELIFT**] Validate 2.1.17 queue
- [x] [**STATUS**] Enable maintenance to drain players + game servers
- [x] [**STATUS**] Make prod-stable API live
- [x] [**STATUS**] Update version check value
- [x] [**TEST**] Validate version check behaving correctly on dev-stable
- [x] [**EGS**] Push patch live
- [x] [**PS5**] Patch scheduled live at 2pm PST
- [x] [**STATUS**] Lift maintenance mode
- [x] [**GITHUB**] Tag v2.1.17 release

# Gamelift Fleet Check
- [x] **us-west-1**
- [x] **us-west-2**
- [x] **us-east-1**
- [x] **us-east-2**
- [x] **eu-central-1**
- [x] **eu-west-1**
- [x] **ap-northeast-1**
- [x] **Queue Validation**

### Fleet Capacity Table
```
Region         Id                                         Type      Desired Min Max Servers Games
us-west-1      fleet-eef035d9-2ec6-44e8-9fa1-5d60847c03bf SPOT      10      10  250 10      9
us-west-2      fleet-b4242740-54e2-4f09-897f-f638d47ab61b SPOT      10      10  500 10      9
us-west-2      fleet-e3fe541a-5ea2-40f1-906f-13bc07acc94b SPOT      10      10  250 20      0
us-east-1      fleet-93db08cc-49ec-405f-8be6-d1bf2bd05fd0 SPOT      25      25  250 25      23
us-east-1      fleet-f5b3b2c3-c603-4242-a5ac-cf61ae458c90 SPOT      25      25  250 50      0
us-east-2      fleet-9625542f-ca57-40b5-b46b-5ed722c999c6 SPOT      10      10  250 10      10
us-east-2      fleet-9a6ede16-ea22-4ff3-8e21-0b602a75cc2f SPOT      10      10  250 20      0
ca-central-1   fleet-9e1e1a8c-80e1-447c-a03b-6de3a68906bf SPOT      1       0   1   2       0
ca-central-1   fleet-e13bb26f-9fc6-459f-a228-adc22bdb8680 SPOT      1       0   1   1       0
eu-west-1      fleet-11f4ce2f-fd30-44ff-8c80-eecb94ad6134 SPOT      25      25  250 31      27
eu-central-1   fleet-30723cf6-32f6-4189-8c51-fdd567498d2b SPOT      25      25  250 64      56
eu-central-1   fleet-59a43910-d20a-481f-a326-7d365da15b36 SPOT      25      25  250 25      0
ap-southeast-1 fleet-00db32c0-38dc-406c-9207-813b3a78ad70 SPOT      1       0   1   2       0
ap-southeast-1 fleet-69e9b12b-c925-426d-8ef5-0956bff0f1a3 SPOT      1       0   1   1       0
ap-southeast-2 fleet-5678c31d-7f12-4f30-b23f-d38be26381e1 SPOT      1       0   1   0       0
ap-southeast-2 fleet-c3f88c7c-eeca-44a6-a18e-f0fc26d80ebb SPOT      1       0   1   1       0
ap-northeast-1 fleet-c01d8436-afdc-4907-ae79-53ec619c476f SPOT      10      10  250 20      0
ap-northeast-1 fleet-f70f2d95-a39a-4c8b-ab8d-edc7bbc9b1aa SPOT      10      10  500 10      0
us-west-2      fleet-3d02d78b-1b90-4de6-995f-a1a5b0a1cda0 ON_DEMAND 10      10  100 20      2
us-east-1      fleet-1bdc4ab9-4749-4859-b039-23c18000396b ON_DEMAND 10      10  250 19      16
us-east-2      fleet-7837f611-1b9b-468b-90a5-ece88115b05f ON_DEMAND 10      10  100 20      4
ca-central-1   fleet-a3553cc4-2d2a-4234-a78a-4fd9a4b55c40 ON_DEMAND 1       0   1   2       0
eu-central-1   fleet-1cdc9ac6-ae8a-49cb-a969-9f9eb74c1547 ON_DEMAND 10      10  100 19      15
ap-southeast-1 fleet-df2fb2b0-961f-440c-b899-6b3eee286c5f ON_DEMAND 1       0   1   2       0
ap-southeast-2 fleet-e947a89e-2597-4b7c-a993-3c663ee24d1d ON_DEMAND 1       0   1   2       0
ap-northeast-1 fleet-39f81d61-1bd0-4fde-8db6-2476e4db3dbc ON_DEMAND 10      10  250 20      0
```