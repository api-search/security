---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Cloudminds Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudMinds declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CloudMinds
provider_slug: cloudminds
scheme_count: 0
schemes: []
slug: cloudminds-authentication
source_filename: cloudminds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: derived\nsource: grpc/harix/**/*.proto, harix 1.0.9 SDK client code (PyPI sdist)\nnote: >-\n  CloudMinds publishes no public authentication documentation — the HARIX RDK developer portal does not\n  answer from outside China and there is no OpenAPI with securitySchemes to read. This profile is derived\n  from the provider's own compiled protobuf descriptors and the first-party Python SDK. It records what\n  the shipped contract actually does, which is a finding in itself: there is no credential scheme on the\n  wire.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  transport_security: none\n  identity_model: identifiers-in-payload\nschemes: []\nfindings:\n- id: no-transport-security\n  severity: high\n  detail: >-\n    Every stub in the SDK is built with grpc.insecure_channel(...) — plaintext HTTP/2. No\n    grpc.ssl_channel_credentials, no call credentials, no channel credentials appear anywhere in\n    harix 1.0.9. Any deployment\
  \ following the first-party SDK carries robot control commands\n    (Move, Rotate, EmergencyStop, ShutdownRobot, RebootRcu) and biometric vision payloads (face,\n    face attributes, face comparison) unencrypted.\n  evidence: harix/rdk/skill/robot_control_api.py, harix/rdk/subscribe/subscribe.py and every other client module\n- id: no-credential-on-the-wire\n  severity: high\n  detail: >-\n    No RPC takes a token, key, signature or authorization field, and no gRPC metadata is attached by\n    the SDK. Caller identity is asserted, not proven — it is carried as plain strings in\n    common.CommonReqInfo (tenant_id, user_id, robot_id, robot_type, service_code). Authorization is\n    therefore entirely the responsibility of the network boundary in front of the gRPC ingress; the\n    published contract has none.\n  evidence: grpc/harix/common/common.proto\n- id: authority-header-as-routing\n  severity: info\n  detail: >-\n    The only channel option the SDK sets is grpc.default_authority,\
  \ supplied by the integrator. That\n    overrides the HTTP/2 :authority pseudo-header, which is a routing/virtual-host selector at the\n    ingress — not an authentication mechanism, though it is the closest thing to a tenant selector in\n    the transport layer.\n  evidence: harix/rdk/**/__init__ channel construction\n- id: app-key-secret-issued-to-callbacks\n  severity: medium\n  detail: >-\n    The one credential pair that appears anywhere in the contract flows the OTHER direction: when HARIX\n    calls a skill application's Vision/BeforeRecognize callback, the application answers with\n    serviceapp.VisionResponse.Propose { do_recognize, app_key, app_secret, faceset_id } — i.e. the skill\n    app hands HARIX the credentials for a third-party recognition service to use on its behalf. Those\n    fields are transported over the same plaintext channel.\n  evidence: grpc/harix/serviceapp/recognizeVision.proto\nidentity_fields:\n- {field: tenant_id, message: common.CommonReqInfo, role:\
  \ tenant}\n- {field: user_id, message: common.CommonReqInfo, role: end user}\n- {field: robot_id, message: common.CommonReqInfo, role: device}\n- {field: robot_type, message: common.CommonReqInfo, role: device model}\n- {field: service_code, message: common.CommonReqInfo, role: calling service}\nscopes:\n  published: false\n  note: No OAuth surface, so no scopes/ artifact is emitted (per pipeline, scopes/ is OAuth-only).\ndocs: null\ndocs_note: >-\n  The developer portal that would document authentication —\n  https://harix.dataarobotics.com/#/index/community/home, linked as \"DEVELOPERS\" from the company's own\n  English homepage — does not complete a TCP connection from a US vantage point (probed 2026-08-10).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudminds/refs/heads/main/authentication/cloudminds-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Frontier Tech
- Robotics
- Cloud Robotics
- Artificial Intelligence
- Robot Development Kit
- HARIX
- gRPC
- Protobuf
- Robot Operating System
- Computer-Vision
- Speech Recognition
---
