---
api_key_in:
- request signature
auth_types:
- apiKey-signature
- mqtt-credentials
- subscription-signature
description: Authentication profile for the Univers EnOS platform APIs, assembled from the first-party SDKs on the EnvisionIot GitHub org and the EnOS API documentation (the docs host itself was unreachable from the probe location; SDK sources are the verified evidence). No OpenAPI document is published, so this profile is searched rather than derived from securitySchemes.
kind: authentication
layout: security
method: searched
name: Univers Authentication
name_suffix: Authentication
oauth_flows: []
overview: Univers secures its APIs with apiKey-signature, mqtt-credentials, and subscription-signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Univers
provider_slug: univers
scheme_count: 3
schemes:
- description: Applications are registered in the EnOS Application Portal / Developer Console to obtain an application accessKey and secretKey. Every EnOS Open API request is signed with these credentials; the service SDKs (com.envisioniot:enos-api for Java, enos-api-sdk-python and enos-poseidon for Python) generate the API request signature automatically and assemble the request URL against the per-environment API gateway address.
  name: EnOS service API request signing
  sources:
  - https://github.com/EnvisionIot/enos-api-sdk-java
  - https://github.com/EnvisionIot/enos-api-sdk-python
  - https://pypi.org/project/enos-poseidon/
  style: accessKey + secretKey HMAC-style request signature
  type: apiKey
- description: Devices connect to EnOS Cloud through the MQTT or HTTP device SDKs using per-device credentials (product key, device key, device secret), with optional X.509 device certificates issued by the EnOS certificate service to secure device-to-cloud communication.
  name: EnOS device connectivity (MQTT/HTTP device secrets)
  sources:
  - https://github.com/EnvisionIot/enos-device-sdk-python
  - https://github.com/EnvisionIot/enos-device-sdk-java
  - https://github.com/EnvisionIot/enos-cert-tool
  style: productKey/deviceKey/deviceSecret over MQTT or HTTP
  type: apiKey
- description: The data-subscription streaming protocol authenticates consumers with an AuthReq protobuf message carrying accessKey, subId, and a sign field (see grpc/univers-enos-subscription-sub.proto, harvested verbatim from the first-party Python subscription SDK).
  name: EnOS data subscription authentication
  sources:
  - https://github.com/EnvisionIot/enos-subscription-service-sdk-python
  style: accessKey + subscription id + signature (protobuf AuthReq)
  type: apiKey
slug: univers-authentication
source_filename: univers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/EnvisionIot\ndocs: https://support.enos-iot.com/docs/api/en/3.0.0/overview.html\ndescription: >-\n  Authentication profile for the Univers EnOS platform APIs, assembled from the\n  first-party SDKs on the EnvisionIot GitHub org and the EnOS API documentation\n  (the docs host itself was unreachable from the probe location; SDK sources\n  are the verified evidence). No OpenAPI document is published, so this profile\n  is searched rather than derived from securitySchemes.\nsummary:\n  types: [apiKey-signature, mqtt-credentials, subscription-signature]\n  api_key_in: [request signature]\n  oauth2_flows: []\nschemes:\n  - name: EnOS service API request signing\n    type: apiKey\n    style: accessKey + secretKey HMAC-style request signature\n    description: >-\n      Applications are registered in the EnOS Application Portal / Developer\n      Console to obtain an application accessKey and secretKey. Every EnOS\n\
  \      Open API request is signed with these credentials; the service SDKs\n      (com.envisioniot:enos-api for Java, enos-api-sdk-python and\n      enos-poseidon for Python) generate the API request signature\n      automatically and assemble the request URL against the per-environment\n      API gateway address.\n    sources:\n      - https://github.com/EnvisionIot/enos-api-sdk-java\n      - https://github.com/EnvisionIot/enos-api-sdk-python\n      - https://pypi.org/project/enos-poseidon/\n  - name: EnOS device connectivity (MQTT/HTTP device secrets)\n    type: apiKey\n    style: productKey/deviceKey/deviceSecret over MQTT or HTTP\n    description: >-\n      Devices connect to EnOS Cloud through the MQTT or HTTP device SDKs using\n      per-device credentials (product key, device key, device secret), with\n      optional X.509 device certificates issued by the EnOS certificate\n      service to secure device-to-cloud communication.\n    sources:\n      - https://github.com/EnvisionIot/enos-device-sdk-python\n\
  \      - https://github.com/EnvisionIot/enos-device-sdk-java\n      - https://github.com/EnvisionIot/enos-cert-tool\n  - name: EnOS data subscription authentication\n    type: apiKey\n    style: accessKey + subscription id + signature (protobuf AuthReq)\n    description: >-\n      The data-subscription streaming protocol authenticates consumers with an\n      AuthReq protobuf message carrying accessKey, subId, and a sign field\n      (see grpc/univers-enos-subscription-sub.proto, harvested verbatim from\n      the first-party Python subscription SDK).\n    sources:\n      - https://github.com/EnvisionIot/enos-subscription-service-sdk-python\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/univers/refs/heads/main/authentication/univers-authentication.yml
summary_line: apiKey-signature/mqtt-credentials/subscription-signature · 3 schemes
tags:
- Company
- Technology
- Energy
- Internet of Things
- Artificial Intelligence
- Sustainability
- Infrastructure
---
