---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 180s.com.br
  spf: true
hosts:
- cert_expires: Sep 30 18:12:09 2026 GMT
  host: 180s.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 180 Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 180 Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 180 Insurance
provider_slug: 180-insurance
slug: 180-insurance-domain-security
source_filename: 180-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 180s.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:12:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 180s.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/security/180-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Insurance
- Embedded Insurance
- Brazil
- Fintech
- API
- Webhooks
---
