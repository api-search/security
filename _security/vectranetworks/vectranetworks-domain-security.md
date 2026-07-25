---
api_specs:
- filename: vectranetworks-accounts-api-openapi.yml
  format: yaml
  label: Vectra AI Accounts API
  slug: vectranetworks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-accounts-api-openapi.yml
- filename: vectranetworks-assignment-outcomes-api-openapi.yml
  format: yaml
  label: Vectra AI Assignment Outcomes API
  slug: vectranetworks-assignment-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-assignment-outcomes-api-openapi.yml
- filename: vectranetworks-assignments-api-openapi.yml
  format: yaml
  label: Vectra AI Assignments API
  slug: vectranetworks-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-assignments-api-openapi.yml
- filename: vectranetworks-detections-api-openapi.yml
  format: yaml
  label: Vectra AI Detections API
  slug: vectranetworks-detections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-detections-api-openapi.yml
- filename: vectranetworks-entities-api-openapi.yml
  format: yaml
  label: Vectra AI Entities API
  slug: vectranetworks-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-entities-api-openapi.yml
- filename: vectranetworks-events-api-openapi.yml
  format: yaml
  label: Vectra AI Events API
  slug: vectranetworks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-events-api-openapi.yml
- filename: vectranetworks-groups-api-openapi.yml
  format: yaml
  label: Vectra AI Groups API
  slug: vectranetworks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-groups-api-openapi.yml
- filename: vectranetworks-health-api-openapi.yml
  format: yaml
  label: Vectra AI Health API
  slug: vectranetworks-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-health-api-openapi.yml
- filename: vectranetworks-hosts-api-openapi.yml
  format: yaml
  label: Vectra AI Hosts API
  slug: vectranetworks-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-hosts-api-openapi.yml
- filename: vectranetworks-lockdown-api-openapi.yml
  format: yaml
  label: Vectra AI Lockdown API
  slug: vectranetworks-lockdown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-lockdown-api-openapi.yml
- filename: vectranetworks-match-api-openapi.yml
  format: yaml
  label: Vectra AI Match API
  slug: vectranetworks-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-match-api-openapi.yml
- filename: vectranetworks-notes-api-openapi.yml
  format: yaml
  label: Vectra AI Notes API
  slug: vectranetworks-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-notes-api-openapi.yml
- filename: vectranetworks-proxies-api-openapi.yml
  format: yaml
  label: Vectra AI Proxies API
  slug: vectranetworks-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-proxies-api-openapi.yml
- filename: vectranetworks-search-api-openapi.yml
  format: yaml
  label: Vectra AI Search API
  slug: vectranetworks-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-search-api-openapi.yml
- filename: vectranetworks-tagging-api-openapi.yml
  format: yaml
  label: Vectra AI Tagging API
  slug: vectranetworks-tagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-tagging-api-openapi.yml
- filename: vectranetworks-threat-feeds-api-openapi.yml
  format: yaml
  label: Vectra AI Threat Feeds API
  slug: vectranetworks-threat-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-threat-feeds-api-openapi.yml
- filename: vectranetworks-users-api-openapi.yml
  format: yaml
  label: Vectra AI Users API
  slug: vectranetworks-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vectra.ai
  spf: true
hosts:
- cert_expires: Oct  2 15:47:38 2026 GMT
  host: www.vectra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: platform.vectra.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Vectranetworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vectra AI, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vectra AI
provider_slug: vectranetworks
slug: vectranetworks-domain-security
source_filename: vectranetworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vectra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:47:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.vectra.ai\n  https: false\ndomains:\n- domain: vectra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/security/vectranetworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Network Detection and Response
- Threat Detection
- Security Operations
- Artificial Intelligence
- SIEM
---
