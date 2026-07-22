---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kendrascott.com
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: kendrascott.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kendrascott Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kendra Scott, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kendra Scott
provider_slug: kendrascott
slug: kendrascott-domain-security
source_filename: kendrascott-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kendrascott.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: kendrascott.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kendrascott/refs/heads/main/security/kendrascott-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Jewelry
- Ecommerce
- Consumer
- Accessories
---
