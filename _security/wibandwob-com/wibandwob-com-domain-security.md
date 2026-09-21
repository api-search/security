---
api_specs:
- filename: wibandwob-com-scramble-openapi.yml
  format: yaml
  label: Scramble API
  slug: scramble-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wibandwob-com/refs/heads/main/openapi/wibandwob-com-scramble-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wibandwob.com
  spf: true
hosts:
- cert_expires: Oct 27 10:00:32 2026 GMT
  host: wibandwob.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 15:45:26 2026 GMT
  host: scramble.wibandwob.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Wibandwob Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wib&Wob (symbients), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wib&Wob (symbients)
provider_slug: wibandwob-com
slug: wibandwob-com-domain-security
source_filename: wibandwob-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wibandwob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 10:00:32 2026 GMT\n  hsts: false\n- host: scramble.wibandwob.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 15:45:26 2026 GMT\n  hsts: false\ndomains:\n- domain: wibandwob.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wibandwob-com/refs/heads/main/security/wibandwob-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agents
- A2A
- x402
- Micropayments
- USDC
- Base
- Art
- ASCII Art
- Generative Art
- Symbients
- AI Agents
- llms-txt
---
