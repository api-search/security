---
api_specs:
- filename: shapelessai-openapi-generated.yml
  format: yaml
  label: ShapelessAI API
  slug: shapelessai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/openapi/_ae-authored/shapelessai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shapelessai.com
  spf: true
hosts:
- cert_expires: Dec 27 13:13:34 2026 GMT
  host: shapelessai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shapelessai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShapelessAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShapelessAI
provider_slug: shapelessai
slug: shapelessai-domain-security
source_filename: shapelessai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shapelessai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 13:13:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shapelessai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shapelessai/refs/heads/main/security/shapelessai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Social Media
- Automation
- SaaS
---
