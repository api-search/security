---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Datavisor Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataVisor secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DataVisor
provider_slug: datavisor
scheme_count: 2
schemes:
- applies_to:
  - DataVisor dEdge Device Intelligence WebAPI
  description: DataVisor secures dEdge data access with access keys, alongside IP allowlisting, white-box encryption and HTTPS. The location (header vs query) and the parameter name are not published on any public page.
  evidence:
    quote: '"DataVisor also uses access keys, IP whitelisting, white-box encryption and HTTPs to further secure data access."'
    url: https://www.datavisor.com/integrations/datavisor-integration-guide-for-device-intelligence
  in: unpublished
  name: access-key
  parameter_name: unpublished
  type: apiKey
- applies_to:
  - DataVisor dEdge Device Intelligence WebAPI
  description: The dEdge SDK initializes on device, sends encrypted device information to the dEdge server, and receives a device token. That token is the identifier the client then presents when querying the dEdge server WebAPI for device signals. DataVisor states it runs an internal algorithm to verify tokens so that forged tokens are rejected. This is a resource identifier bound to a device rather than a general-purpose API credential.
  evidence:
    quote: '"All data is encrypted and sent to dEdge server, which returns a token for that device that you can use to query the dEdge server for device-specific information" ... "dEdge has an internal algorithm to verify tokens, so that hackers cannot fake our tokens."'
    url: https://www.datavisor.com/integrations/datavisor-integration-guide-for-device-intelligence
  name: device-token
  type: bearer-like-token
slug: datavisor-authentication
source_filename: datavisor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: DataVisor public integration guides and API references page\ndocs: https://www.datavisor.com/datavisor-api-guide\nnote: >-\n  DataVisor publishes no OpenAPI or Swagger definition anonymously, so this profile could\n  not be derived mechanically. It is assembled only from the authentication and transport\n  security statements DataVisor makes on its own public integration pages. Exact header\n  names, parameter names and token formats are NOT published publicly and are therefore\n  not recorded here; they are issued per customer by a DataVisor technical account manager\n  and documented in the gated API guide.\nsummary:\n  types:\n  - apiKey\n  key_material:\n  - access key\n  - device token\n  network_controls:\n  - ip-allowlist\n  transport:\n    protocol: HTTPS\n    minimum_tls: TLSv1.2\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: access-key\n  type: apiKey\n  applies_to:\n  - DataVisor\
  \ dEdge Device Intelligence WebAPI\n  in: unpublished\n  parameter_name: unpublished\n  description: >-\n    DataVisor secures dEdge data access with access keys, alongside IP allowlisting,\n    white-box encryption and HTTPS. The location (header vs query) and the parameter\n    name are not published on any public page.\n  evidence:\n    url: https://www.datavisor.com/integrations/datavisor-integration-guide-for-device-intelligence\n    quote: >-\n      \"DataVisor also uses access keys, IP whitelisting, white-box encryption and HTTPs\n      to further secure data access.\"\n- name: device-token\n  type: bearer-like-token\n  applies_to:\n  - DataVisor dEdge Device Intelligence WebAPI\n  description: >-\n    The dEdge SDK initializes on device, sends encrypted device information to the dEdge\n    server, and receives a device token. That token is the identifier the client then\n    presents when querying the dEdge server WebAPI for device signals. DataVisor states it\n    runs an internal\
  \ algorithm to verify tokens so that forged tokens are rejected. This is\n    a resource identifier bound to a device rather than a general-purpose API credential.\n  evidence:\n    url: https://www.datavisor.com/integrations/datavisor-integration-guide-for-device-intelligence\n    quote: >-\n      \"All data is encrypted and sent to dEdge server, which returns a token for that\n      device that you can use to query the dEdge server for device-specific information\"\n      ... \"dEdge has an internal algorithm to verify tokens, so that hackers cannot fake\n      our tokens.\"\nnetwork_controls:\n- control: ip-allowlist\n  applies_to:\n  - DataVisor dEdge Device Intelligence WebAPI\n  evidence: https://www.datavisor.com/integrations/datavisor-integration-guide-for-device-intelligence\ntransport_security:\n  protocol: HTTPS\n  minimum_tls: TLSv1.2\n  evidence:\n    url: https://www.datavisor.com/datavisor-api-guide\n    quote: >-\n      \"The default integration mechanism for all APIs supports\
  \ real-time, synchronous\n      HTTPS-based RESTful calls (secured with TLS v1.2).\"\n  encryption_at_rest: true\n  encryption_at_rest_evidence:\n    url: https://www.datavisor.com/integrations/datavisor-integration-guide-for-comprehensive-fraud-solution\n    quote: >-\n      \"We secure data transmission by providing advanced encryption at rest and supporting\n      HTTPS for real-time data transfers.\"\ntenancy:\n  model: dedicated-per-customer\n  evidence:\n    url: https://www.datavisor.com/integrations/datavisor-integration-guide-for-comprehensive-fraud-solution\n    quote: >-\n      \"For every client, we implement the detection system to dedicated cloud machines,\n      making sure that your data is only visible and accessible to you.\"\ngaps:\n- No public authentication reference page; no header/parameter names published.\n- No OAuth 2.0, OpenID Connect or mutual TLS surface documented publicly.\n- No public self-service credential issuance; keys are provisioned by a technical\
  \ account manager.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavisor/refs/heads/main/authentication/datavisor-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Fraud Detection
- Fraud Prevention
- Anti-Money Laundering
- Financial Crime
- Risk Management
- Machine Learning
- Artificial Intelligence
- Device Intelligence
- Banking
- Payments
- Compliance
---
