---
api_specs:
- filename: payer-openapi-generated.yml
  format: yaml
  label: Payer API
  slug: payer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/openapi/_ae-authored/payer-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: payer.eu
  spf: false
hosts:
- cert_expires: Nov 26 22:06:43 2026 GMT
  host: payer.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Payer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Payer
provider_slug: payer
slug: payer-domain-security
source_filename: payer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payer.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 22:06:43 2026 GMT\n  hsts: false\ndomains:\n- domain: payer.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payer/refs/heads/main/security/payer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- B2B
- FinTech
- Automation
---
