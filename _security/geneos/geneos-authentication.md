---
anonymous_access: false
api_key_in: []
api_specs:
- filename: geneos-rest-api-api-openapi.yml
  format: yaml
  label: Geneos REST API
  slug: geneos-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geneos/refs/heads/main/openapi/geneos-rest-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Geneos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geneos declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Geneos
provider_slug: geneos
scheme_count: 0
schemes: []
slug: geneos-authentication
source_filename: geneos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  https://docs.itrsgroup.com/docs/geneos/current/processing/monitoring-and-alerts/geneos_commands_tr/index.html#user-authentication\ndocs:\n  - >-\n    https://docs.itrsgroup.com/docs/geneos/current/processing/monitoring-and-alerts/geneos_commands_tr/index.html#user-authentication\n  - https://docs.itrsgroup.com/docs/geneos/current/collection/rest-api/index.html#plugin-configuration\n  - https://docs.itrsgroup.com/docs/geneos/current/collection/xml-rpc-api/index.html\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Geneos\nproviderId: geneos\nnote: >-\n  derive-authentication.py produced nothing for this provider because the one\n  published OpenAPI declares no securitySchemes at all. Everything below was\n  read from ITRS Group's own documentation. Geneos is customer-deployed, so\n  every authentication decision here is a deployment choice the customer makes,\n  not a property of a hosted\
  \ service — and in two of the three surfaces the\n  default is no authentication.\nsummary:\n  oauth2: false\n  openid_connect: false\n  api_keys: false\n  http_basic: true\n  bearer_token: true\n  mutual_tls: true\n  sso: true\n  unauthenticated_default: true\nsurfaces:\n  - api: geneos:gateway-rest\n    name: Geneos Gateway REST Command Service\n    enabled_by_default: false\n    schemes:\n      - id: gatewayBasic\n        type: http\n        scheme: basic\n        description: >-\n          \"For password-based authentication, each REST command must be\n          accompanied by a username and password, using HTTP basic access\n          authentication.\" Credentials are users configured with passwords in the\n          Gateway setup. ITRS warns in the same section that the header is\n          base64-encoded but neither encrypted nor hashed, and recommends\n          restricting the REST service to secure connections when authentication\n          is enabled.\n        evidence: >-\n\
  \          https://docs.itrsgroup.com/docs/geneos/current/processing/monitoring-and-alerts/geneos_commands_tr/index.html#user-authentication\n      - id: gatewaySsoBearer\n        type: http\n        scheme: bearer\n        description: >-\n          An SSO access token supplied as `Authorization: Bearer <token>`.\n          Obtained from `GET /rest/authorize`, which redirects the HTTP client to\n          the configured SSO Agent; if the SSO provider is ITRS Analytics a\n          different token flow applies. Tokens expire and a new one must then be\n          obtained. The Gateway refuses SSO-token connections unless the SSO\n          Agent setting is present.\n        token_endpoint: '{gatewayHost}:{restPort}/rest/authorize'\n        evidence: >-\n          https://docs.itrsgroup.com/docs/geneos/current/processing/monitoring-and-alerts/geneos_commands_tr/index.html#user-authentication\n    not_supported:\n      - >-\n        System logins. \"System logins are not supported, since\
  \ system credentials\n        are checked by the user interface client (e.g. Active Console), which is\n        not involved in the REST API.\"\n    authorization:\n      model: per-command, per-target permissions\n      description: >-\n        403 is returned both for invalid credentials and for valid credentials\n        without permission to run the requested command on the requested target.\n        /rest/commands/available and /rest/xpaths/commandTargets filter their\n        results by the caller's permissions; /rest/commands/all and\n        /rest/xpaths/match deliberately do not.\n    transport:\n      https_supported: true\n      https_enforceable: true\n      setting: commands > restService > allowOnInsecureComms\n      description: >-\n        The REST service can be configured to run only on secure connections. A\n        request made on the insecure port while the service is secure returns 404.\n  - api: geneos:netprobe-rest-api\n    name: Geneos Netprobe REST API\n    enabled_by_default:\
  \ true\n    schemes:\n      - id: netprobeMutualTLS\n        type: mutualTLS\n        optional: true\n        description: >-\n          The plug-in can require clients to present a valid certificate by\n          enabling \"Verify client certificate\" and supplying a \"Client CA\n          certificate\" path; if the path is empty the plug-in falls back to the\n          Netprobe's -ssl-certificate-chain file and logs a warning. HTTPS\n          requires starting the Netprobe with -secure, -ssl-certificate and\n          -ssl-certificate-key.\n        evidence: https://docs.itrsgroup.com/docs/geneos/current/collection/rest-api/index.html#plugin-configuration\n    gap: >-\n      The published OpenAPI declares no securitySchemes and no security\n      requirement, so a client generated from the contract will send\n      unauthenticated requests. With mutual TLS not configured, anything that can\n      reach port 7136 can create, update and delete dataviews and rows.\n  - api: geneos:xml-rpc\n\
  \    name: Geneos XML-RPC Instrumentation API\n    enabled_by_default: true\n    schemes: []\n    description: >-\n      \"XML-RPC traffic is neither encrypted or authenticated.\" ITRS documents\n      IPSec as the suggested mitigation. Access control is a host allow-list:\n      TRUSTED_API_HOSTS, set as an environment variable or in the managed entity\n      descriptor, is a comma-separated list of trusted hosts/IPs; calls from any\n      other host return HOST_NOT_TRUSTED immediately and the first such call from\n      each host is written to the Netprobe log. If the Netprobe runs in secure\n      mode the XML-RPC client must use HTTPS as the transport.\n    evidence: https://docs.itrsgroup.com/docs/geneos/current/collection/xml-rpc-api/index.html\nscopes:\n  published: false\n  note: >-\n    No OAuth 2.0 flow and therefore no scope surface. scopes/ is deliberately not\n    written for this provider — permissions are Gateway user permissions on\n    commands and targets, not OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geneos/refs/heads/main/authentication/geneos-authentication.yml
summary_line: 0 schemes
tags:
- APM
- Capital Markets
- Infrastructure
- ITRS
- Monitoring
- Observability
- Real-Time
- Trading Systems
- XML-RPC
- OpenAPI
---
