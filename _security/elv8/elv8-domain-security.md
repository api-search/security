---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scout-financial.com
  spf: false
hosts:
- cert_expires: Sep 16 07:01:52 2026 GMT
  host: www.scout-financial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elv8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ELV8, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ELV8
provider_slug: elv8
slug: elv8-domain-security
source_filename: elv8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scout-financial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scout-financial.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elv8/refs/heads/main/security/elv8-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial Services
- NIL
- College Athletics
- Payments
- Investment Advisory
- Compliance
---
