---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: none
name: Metricstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: MetricStream declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: MetricStream
provider_slug: metricstream
scheme_count: 0
schemes: []
slug: metricstream-authentication
source_filename: metricstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: none\nsource: MetricStream Business API module overview pages (https://assets.metricstream.com/pdf/Developer-Portal/MsIsmISM-API-Overview.html\n  and siblings), the 34 reference pages under https://assets.metricstream.com/pdf/Developer-Portal/, the platform\n  APIs page https://www.metricstream.com/platform/apis.htm, and /.well-known/ probes on every MetricStream host\n  — all read 2026-08-25.\nsummary: MetricStream's public API documentation confirms that its Business REST APIs are AUTHENTICATED and that\n  authorization is activity-based, but it does not publish WHICH authentication scheme to use. No securityScheme\n  is declared (there is no machine-readable spec), no Authorization header is shown in any of the 204 rendered curl\n  samples, no token endpoint is named, and no OpenID/OAuth discovery document is served on any host. The scheme\n  is obtainable only from MetricStream Support or the gated partner portal.\nscheme_count: 0\nschemes:\
  \ []\ndocumented_facts:\n- fact: Authentication is required.\n  evidence: Every one of the 204 published operations declares \"401 - Required Authentication information is missing\n    or invalid.\"\n  source: https://assets.metricstream.com/pdf/Developer-Portal/GRCF_API/MsGrcRisk.html\n- fact: The APIs let customers \"make authenticated calls against core features\" from other applications.\n  source: https://assets.metricstream.com/pdf/Developer-Portal/MsIsmISM-API-Overview.html\n- fact: Authorization is built in for the REST endpoints \"using activities, to prevent unauthorized access\".\n  evidence: 403 Forbidden - Insufficient user privileges is declared on all 204 operations.\n  source: https://assets.metricstream.com/pdf/Developer-Portal/MsIsmISM-API-Overview.html\n- fact: Alternate authentication schemes exist but are not published.\n  evidence: '\"For more advanced usages of Integration, such as using alternate Authentication Schemes OR other functional\n    needs, contact MetricStream\
  \ Support team.\"'\n  source: https://assets.metricstream.com/pdf/Developer-Portal/MsIsmISM-API-Overview.html\n- fact: Transport is TLS and clients are told to validate the server certificate.\n  source: https://assets.metricstream.com/pdf/Developer-Portal/GRCF_API/MsGrcGRC%20API%20Overview.html\n- fact: MetricStream markets \"appropriate security and authentication wrappers\" on its OpenAPI-compliant REST APIs.\n  source: https://www.metricstream.com/platform/apis.htm\nnegative_probes:\n- url: https://www.metricstream.com/.well-known/openid-configuration\n  status: 404\n- url: https://www.metricstream.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://www.metricstream.com/.well-known/oauth-protected-resource\n  status: 404\n- url: https://assets.metricstream.com/.well-known/openid-configuration\n  status: 404\n- url: https://info.metricstream.com/.well-known/openid-configuration\n  status: 404\noauth:\n  declared: false\n  note: No OAuth 2.0 or OpenID Connect surface\
  \ is documented or discoverable, so no scopes/ artifact is written\n    — this is a key/credential API with no published scope vocabulary, and forcing an empty scopes file would misrepresent\n    it.\ngap: This is the highest-value, lowest-cost fix on MetricStream's public API surface. A single page naming the scheme\n  (header name, credential type, how to obtain it, token lifetime) would let a developer or an agent get from the\n  published 204-operation reference to a first successful call. Today the reference is complete enough to plan an\n  integration and stops one step short of making one.\nmethod_note: No authentication scheme is published (schemes empty); documented facts retained.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metricstream/refs/heads/main/authentication/metricstream-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Governance
- Risk Management
- Compliance
- GRC
- Audit
- Enterprise Software
- RegTech
- Cyber Risk
- Third-Party Risk Management
- Operational Resilience
- ESG
---
