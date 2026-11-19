This is a Postman Collections for the DIDWW API3 endpoints for different versions:

* 2017-09-18
* 2021-04-19
* 2021-12-15
* 2022-05-10
* 2026-04-16
* 2026-11-19 (Latest)

Refer to the main [DIDWW API documentation](https://doc.didww.com/api3/index.html) for more details.

## Installation

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/58791732-d5471fb4-12ea-48a2-81d3-26604bebe70c?action=collection%2Ffork&collection-url=entityId%3D58791732-d5471fb4-12ea-48a2-81d3-26604bebe70c%26entityType%3Dcollection%26workspaceId%3Dc7e9c67d-ac71-4c91-a5ef-b12f6619f415#?env%5BDIDWW%20Sandbox%5D=W3sia2V5IjoiaG9zdCIsInZhbHVlIjoic2FuZGJveC1hcGkuZGlkd3cuY29tIiwiZW5hYmxlZCI6dHJ1ZSwic2Vzc2lvblZhbHVlIjoic2FuZGJveC1hcGkuZGlkd3cuY29tIiwic2Vzc2lvbkluZGV4IjowfSx7ImtleSI6InZpbkhvc3QiLCJ2YWx1ZSI6ImFwaS12aW4tc2FuZGJveC5kaWR3dy5jb20iLCJlbmFibGVkIjp0cnVlLCJzZXNzaW9uVmFsdWUiOiJhcGktdmluLXNhbmRib3guZGlkd3cuY29tIiwic2Vzc2lvbkluZGV4IjoxfSx7ImtleSI6InZvdXRIb3N0IiwidmFsdWUiOiJhcGktdm91dC1zYW5kYm94LmRpZHd3LmNvbSIsImVuYWJsZWQiOnRydWUsInNlc3Npb25WYWx1ZSI6ImFwaS12b3V0LXNhbmRib3guZGlkd3cuY29tIiwic2Vzc2lvbkluZGV4IjoyfSx7ImtleSI6InNtc0hvc3QiLCJ2YWx1ZSI6ImFwaS1zbXMtc2FuZGJveC5kaWR3dy5jb20iLCJlbmFibGVkIjp0cnVlLCJzZXNzaW9uVmFsdWUiOiJhcGktc21zLXNhbmRib3guZGlkd3cuY29tIiwic2Vzc2lvbkluZGV4IjozfSx7ImtleSI6ImF1dGhIb3N0IiwidmFsdWUiOiJhdXRoLXNhbmRib3guZGlkd3cuY29tIiwiZW5hYmxlZCI6dHJ1ZSwic2Vzc2lvblZhbHVlIjoiYXV0aC1zYW5kYm94LmRpZHd3LmNvbSIsInNlc3Npb25JbmRleCI6NH0seyJrZXkiOiJhcGlLZXkiLCJ2YWx1ZSI6InlvdXJEaWR3d0FwaUtleSIsImVuYWJsZWQiOnRydWUsInNlc3Npb25WYWx1ZSI6InlvdXJEaWR3d0FwaUtleSIsInNlc3Npb25JbmRleCI6NX1d)

### Manual

You can download these Collections from a GitHub repo here: https://github.com/didww/didww-api3-postman

## Environment

These Collections include pre-configured **DIDWW Sandbox** and **DIDWW Production** Environments. You will need to set up the following variables in order to run each request:

| Name     | Description                                                                                        |
| -------- | -------------------------------------------------------------------------------------------------- |
| `host`   | Environment host. Details [here](https://doc.didww.com/api3/index.html#environments-and-endpoints) |
| `vinHost`, `voutHost`, `smsHost` | Hosts of the inbound call, outbound call and SMS price services (2026-11-19 and later) |
| `authHost` | Host of the token service (2026-11-19 and later) |
| `apiKey` | DIDWW API key. How to receive API key [read here](https://doc.didww.com/api3/index.html#api-keys)  |

The collections up to 2026-04-16 send `apiKey` in the `Api-Key` header and use only `host` and `apiKey`. Starting with 2026-11-19, the collection mints a bearer access token from `apiKey` with `POST https://{{authHost}}/token` and sends it with every request. Put your API key into the *current value* of `apiKey`.
