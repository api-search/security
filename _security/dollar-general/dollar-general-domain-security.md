---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dollargeneral.com
  spf: true
hosts:
- cert_expires: Oct  5 21:58:15 2026 GMT
  host: www.dollargeneral.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dollar General Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dollar General, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dollar General
provider_slug: dollar-general
slug: dollar-general-domain-security
source_filename: dollar-general-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dollargeneral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:58:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: dollargeneral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dollar-general/refs/heads/main/security/dollar-general-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Discount Retail
- Fortune 500
- Vendor Management
---
