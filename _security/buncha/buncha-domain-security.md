---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gobuncha.com
  spf: true
hosts:
- cert_expires: Oct 12 23:20:44 2026 GMT
  host: www.gobuncha.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buncha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buncha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Buncha
provider_slug: buncha
slug: buncha-domain-security
source_filename: buncha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gobuncha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:20:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: gobuncha.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buncha/refs/heads/main/security/buncha-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E Commerce
- Grocery
- Delivery
- Logistics
- Consumer
- Sustainability
- Retail
---
