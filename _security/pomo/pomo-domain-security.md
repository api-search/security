---
api_specs:
- filename: pomo-openapi.yml
  format: yaml
  label: Pomo Platform API
  slug: pomo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomo/refs/heads/main/openapi/pomo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usepomo.ai
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: usepomo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.usepomo.ai
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pomo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pomo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pomo
provider_slug: pomo
slug: pomo-domain-security
source_filename: pomo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usepomo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.usepomo.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usepomo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pomo/refs/heads/main/security/pomo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- Artificial Intelligence
- Market Intelligence
- Competitive Intelligence
- Marketing Automation
- Generative AI
- Software-as-a-Service
- Answer Engine Optimization
- Advertising
- Social-Media
- Influencer Marketing
- Campaign Management
---
