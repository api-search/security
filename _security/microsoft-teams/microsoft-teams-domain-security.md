---
api_specs:
- filename: microsoft-teams-graph-api.yaml
  format: yaml
  label: Microsoft Graph Teams API
  slug: microsoft-graph-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/openapi/microsoft-teams-graph-api.yaml
- filename: microsoft-teams-asyncapi.yaml
  format: yaml
  label: Microsoft Teams Bot Framework API
  slug: microsoft-teams-bot-framework-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/asyncapi/microsoft-teams-asyncapi.yaml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: trafficmanager.net
  spf: false
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 03:53:00 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 11:22:58 2026 GMT
  host: smba.trafficmanager.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Microsoft Teams Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Teams, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Teams
provider_slug: microsoft-teams
slug: microsoft-teams-domain-security
source_filename: microsoft-teams-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:53:00 2026 GMT\n  hsts: null\n- host: smba.trafficmanager.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 11:22:58 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: trafficmanager.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-teams/refs/heads/main/security/microsoft-teams-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat
- Collaboration
- Communication
- Microsoft 365
- Productivity
- Video Conferencing
---
