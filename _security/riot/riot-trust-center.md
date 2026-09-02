---
api_specs:
- filename: riot-awareness-api-openapi.yml
  format: yaml
  label: Riot Awareness API
  slug: riot-awareness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-awareness-api-openapi.yml
- filename: riot-breaches-api-openapi.yml
  format: yaml
  label: Riot Breaches API
  slug: riot-breaches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-breaches-api-openapi.yml
- filename: riot-general-api-openapi.yml
  format: yaml
  label: Riot General API
  slug: riot-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-general-api-openapi.yml
- filename: riot-groups-api-openapi.yml
  format: yaml
  label: Riot Groups API
  slug: riot-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-groups-api-openapi.yml
- filename: riot-inbox-api-openapi.yml
  format: yaml
  label: Riot Inbox API
  slug: riot-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-inbox-api-openapi.yml
- filename: riot-scim-api-openapi.yml
  format: yaml
  label: Riot SCIM API
  slug: riot-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-scim-api-openapi.yml
- filename: riot-simulation-api-openapi.yml
  format: yaml
  label: Riot Simulation API
  slug: riot-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-simulation-api-openapi.yml
- filename: riot-slash-api-openapi.yml
  format: yaml
  label: Riot Slash API
  slug: riot-slash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-slash-api-openapi.yml
- filename: riot-sonar-api-openapi.yml
  format: yaml
  label: Riot Sonar API
  slug: riot-sonar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-sonar-api-openapi.yml
certifications:
- AICPA SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Riot Trust Center
name_suffix: Trust Center
overview: Riot maintains a public trust center documenting AICPA SOC 2 Type II and GDPR compliance.
provider_name: Riot
provider_slug: riot
slug: riot-trust-center
source_filename: riot-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: true\nsource: https://tryriot.com/security/\nurl: https://trust.tryriot.com/\nplatform: Vanta\nsecurity_page: https://tryriot.com/security/\ncertifications:\n- id: soc2-type-ii\n  name: AICPA SOC 2 Type II\n  source: https://tryriot.com/security/\n- id: gdpr\n  name: GDPR\n  source: https://tryriot.com/security/\nprogram:\n  penetration_testing: annual pentest campaigns\n  vulnerability_disclosure: security/riot-vulnerability-disclosure.yml\n  encryption_at_rest: AES 256\n  encryption_in_transit: TLS 1.2+\n  data_hosting:\n  - AWS (Ireland)\n  - Azure (France)\n  backups: daily encrypted backups, 12-hour RTO, 24-hour RPO\n  access_control:\n  - SSO with leading identity providers\n  - role-based access control\n  - MFA required\n  - annual access reviews\n  sdlc:\n  - peer code review before production\ncontact: security@tryriot.com\nevidence:\n- source: https://trust.tryriot.com/\n  http_status: 200\n  kind: trust center\n\
  \  platform_detected: vanta\n  note: >-\n    The trust center is a client-side-rendered Vanta page; the certification list is fetched by JavaScript\n    and is not present in the served HTML. The certifications above are therefore taken from the\n    server-rendered https://tryriot.com/security/ page, which names them in text.\n- source: https://tryriot.com/security/\n  http_status: 200\n  kind: security page\n  keywords:\n  - AICPA SOC 2 Type II\n  - GDPR\n  - bug bounty\n  - annual pentest campaigns\n  - Trust Center\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/security/riot-trust-center.yml
summary_line: AICPA SOC 2 Type II, GDPR
tags:
- Cybersecurity
- Security Awareness
- Human Risk Management
- Phishing Simulation
- employee-security
- Security Posture Management
- breach-detection
- Email Security
- SaaS Security
- SCIM
- Webhook
- OCSF
- France
trust_url: https://trust.tryriot.com/
---
