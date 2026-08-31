---
api_specs:
- filename: amuncore-dynamic-api-api-openapi.yml
  format: yaml
  label: AmunCore Dynamic API
  slug: amuncore-dynamic-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/openapi/amuncore-dynamic-api-api-openapi.yml
certifications: []
description: 'AmunCore publishes a dedicated, public security and data-protection page written for evaluation — hosting model, per-channel protections, encryption, access control, auditing, and an explicitly labelled "Honest roadmap" of what is not yet implemented. It is a trust page in substance, not a badge wall: it names zero certifications and says so.'
kind: trust-center
layout: security
name: Amuncore Trust Center
name_suffix: Trust Center
overview: AmunCore maintains a public trust center covering its security and compliance posture.
provider_name: AmunCore
provider_slug: amuncore
slug: amuncore-trust-center
source_filename: amuncore-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: searched\nsource: https://amuncore.com/security.html\ndescription: >-\n  AmunCore publishes a dedicated, public security and data-protection page written\n  for evaluation — hosting model, per-channel protections, encryption, access\n  control, auditing, and an explicitly labelled \"Honest roadmap\" of what is not yet\n  implemented. It is a trust page in substance, not a badge wall: it names zero\n  certifications and says so.\ntrust_page: https://amuncore.com/security.html\ncertifications: []\nattestations: []\ncertification_note: >-\n  No SOC 2, ISO 27001, PCI DSS, HIPAA or FedRAMP certification is claimed. The\n  provider states independent penetration testing and ISO 27001 alignment are on\n  the roadmap and not implemented. For regulated buyers it recommends an\n  on-premises install plus a joint security review with the customer's own team.\nhosting_models:\n- model: self-hosted\n  description: >-\n    Install on the customer's own servers\
  \ behind their firewall, connecting to\n    their databases with credentials they control. Data never leaves their\n    environment. Positioned for banks, enterprises and regulated industries.\n- model: managed-cloud\n  description: Hosted platform with strict per-company isolation of applications, endpoints and data.\ndata_handling:\n  copies_customer_records: false\n  statement: >-\n    \"We never copy, export, or store your database records. AmunCore acts as a\n    controlled access layer in front of your data.\"\nchannel_controls:\n- channel: REST API\n  controls: >-\n    Per-application API key on every request; parameterized queries; rate\n    limiting; optional IP whitelisting; full audit logging.\n- channel: GraphQL\n  controls: >-\n    Resolved by application ID plus API key together; per-endpoint authentication;\n    only explicitly exposed fields are queryable.\n- channel: AI / MCP\n  controls: >-\n    Gated by a separate secret token distinct from the REST API keys; scoped\
  \ to a\n    single company; same audit logging; can be disabled entirely per company.\n- channel: Webhooks\n  controls: HMAC-SHA256 signed payloads; delivery attempts logged.\nencryption:\n  at_rest: AES-256 for database connection strings and other secrets, including two-factor secrets.\n  in_transit: HTTPS/TLS; TLSv1.3 and HSTS max-age 2592000 observed live.\n  integrity: License keys and webhook payloads signed with HMAC-SHA256.\naccess_control:\n  password_storage: BCrypt\n  mfa: Optional TOTP 2FA with one-time recovery codes and administrator reset\n  roles: [SuperAdmin, Admin, Developer, Viewer]\n  tenant_isolation: Strict per-company separation enforced on every request\nsql_injection:\n  posture: >-\n    All database access uses fully parameterized queries across table endpoints,\n    stored-procedure endpoints and every supported engine; user input is never\n    concatenated into SQL.\nauditing:\n  request_log_fields: [method, path, status_code, response_time, source_ip]\n  analytics:\
  \ Real-time usage, error-rate and latency analytics\n  webhook_delivery: Delivery attempts and outcomes recorded\npublished_roadmap_gaps:\n- Single sign-on (OAuth2 / SAML) and social login — not implemented\n- Audit-log export to external SIEM systems — not implemented\n- Independent penetration testing and ISO 27001 alignment — not implemented\nvulnerability_disclosure:\n  policy_url: null\n  security_txt: null\n  bug_bounty: null\n  contact: sales@amuncore.com\n  note: >-\n    There is no vulnerability-disclosure policy, no /.well-known/security.txt and\n    no bug-bounty program. The only security contact is the general sales address\n    offered for enterprise review, which is not a disclosure channel — a\n    researcher has no published route to report a finding. No VulnerabilityDisclosure\n    artifact or Security pointer is emitted, because none exists to point at.\ndisclaimer: >-\n  The page states it \"is a summary for evaluation purposes and does not constitute\n  a security\
  \ warranty.\"\nevidence:\n- url: https://amuncore.com/security.html\n  status: 200\n- url: https://amuncore.com/.well-known/security.txt\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amuncore/refs/heads/main/security/amuncore-trust-center.yml
summary_line: trust center published
tags:
- Database
- API Management
- Backend
- No-Code
- SQL
- PostgreSQL
- MySQL
- Oracle
- MCP
- Agents
- Data
- SQL Server
- Webhook
- OpenAPI
- Low-Code
- Egypt
trust_url: ''
---
