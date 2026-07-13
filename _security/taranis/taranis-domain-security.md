---
api_specs:
- filename: taranis-openapi.yml
  format: yaml
  label: Taranis Crop Intelligence
  slug: taranis-crop-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taranis/refs/heads/main/openapi/taranis-openapi.yml
- filename: taranis-openapi.yml
  format: yaml
  label: Taranis Imagery and Insights
  slug: taranis-imagery-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taranis/refs/heads/main/openapi/taranis-openapi.yml
- filename: taranis-openapi.yml
  format: yaml
  label: Taranis Ag Assistant
  slug: taranis-ag-assistant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taranis/refs/heads/main/openapi/taranis-openapi.yml
- filename: taranis-openapi.yml
  format: yaml
  label: Taranis Platform Integrations
  slug: taranis-platform-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taranis/refs/heads/main/openapi/taranis-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: taranis.com
  spf: true
hosts:
- cert_expires: Feb 14 20:42:19 2027 GMT
  host: www.taranis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:55:43 2026 GMT
  host: go.taranis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taranis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taranis, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Taranis
provider_slug: taranis
slug: taranis-domain-security
source_filename: taranis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.taranis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 20:42:19 2027 GMT\n  hsts: false\n- host: go.taranis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:55:43 2026 GMT\n  hsts: false\ndomains:\n- domain: taranis.com\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taranis/refs/heads/main/security/taranis-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Agriculture
- AgTech
- Crop Intelligence
- Computer Vision
- Aerial Scouting
- Precision Agriculture
---
