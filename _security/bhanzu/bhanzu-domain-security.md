---
api_specs:
- filename: bhanzu-ai-api-openapi.yml
  format: yaml
  label: Bhanzu AI API
  slug: bhanzu-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bhanzu/refs/heads/main/openapi/bhanzu-ai-api-openapi.yml
- filename: bhanzu-content-api-openapi.yml
  format: yaml
  label: Bhanzu Content API
  slug: bhanzu-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bhanzu/refs/heads/main/openapi/bhanzu-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bhanzu.com
  spf: true
hosts:
- cert_expires: Apr  4 23:59:59 2027 GMT
  host: bhanzu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bhanzu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bhanzu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bhanzu
provider_slug: bhanzu
slug: bhanzu-domain-security
source_filename: bhanzu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bhanzu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bhanzu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bhanzu/refs/heads/main/security/bhanzu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Math
- E‑learning
- AI
- K‑12
---
