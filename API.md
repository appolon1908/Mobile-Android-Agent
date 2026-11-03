# API wiring

The enrolled Android agent communicates only with authorized platform endpoints.

Calls:
- POST /v1/devices during enrollment
- POST /v1/devices/{device_id}/heartbeat
- GET /v1/devices/{device_id}/commands
- GET /v1/devices/{device_id}/policies
- POST /v1/devices/{device_id}/commands/{command_id}/result

The agent never accepts commands that bypass Android security or third-party authentication.