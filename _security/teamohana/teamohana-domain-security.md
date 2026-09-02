---
api_specs:
- filename: teamohana-discovery-api-openapi.yml
  format: yaml
  label: TeamOhana Discovery API
  slug: teamohana-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamohana/refs/heads/main/openapi/teamohana-discovery-api-openapi.yml
- filename: teamohana-headcount-api-openapi.yml
  format: yaml
  label: TeamOhana Headcount API
  slug: teamohana-headcount-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamohana/refs/heads/main/openapi/teamohana-headcount-api-openapi.yml
- filename: teamohana-scenario-api-openapi.yml
  format: yaml
  label: TeamOhana Scenario API
  slug: teamohana-scenario-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamohana/refs/heads/main/openapi/teamohana-scenario-api-openapi.yml
- filename: teamohana-scim-api-openapi.yml
  format: yaml
  label: TeamOhana SCIM API
  slug: teamohana-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teamohana/refs/heads/main/openapi/teamohana-scim-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teamohana.com
  spf: true
hosts:
- cert_expires: Oct  1 05:17:11 2026 GMT
  host: teamohana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teamohana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeamOhana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TeamOhana
provider_slug: teamohana
slug: teamohana-domain-security
source_filename: teamohana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teamohana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:17:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: teamohana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamohana/refs/heads/main/security/teamohana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- HR Tech
- Headcount Management
- Headcount Planning
- Workforce Planning
- Human Resources
- Talent Acquisition
- Finance
- SCIM
- Software-as-a-Service
---
