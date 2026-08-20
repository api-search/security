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
- filename: riot-team-awareness-api-openapi.yml
  format: yaml
  label: Riot Team awareness API
  slug: riot-team-awareness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-team-awareness-api-openapi.yml
- filename: riot-team-inbox-api-openapi.yml
  format: yaml
  label: Riot Team inbox API
  slug: riot-team-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-team-inbox-api-openapi.yml
- filename: riot-team-platform-api-openapi.yml
  format: yaml
  label: Riot Team platform API
  slug: riot-team-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-team-platform-api-openapi.yml
- filename: riot-team-simulation-api-openapi.yml
  format: yaml
  label: Riot Team simulation API
  slug: riot-team-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-team-simulation-api-openapi.yml
- filename: riot-webhook-events-api-openapi.yml
  format: yaml
  label: Riot Webhook Events API
  slug: riot-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/openapi/riot-webhook-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryriot.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: tryriot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 06:25:31 2026 GMT
  host: docs.tryriot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: public-api.tryriot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riot, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Riot
provider_slug: riot
slug: riot-domain-security
source_filename: riot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryriot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tryriot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:25:31 2026 GMT\n  hsts: false\n- host: public-api.tryriot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tryriot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riot/refs/heads/main/security/riot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
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
---
