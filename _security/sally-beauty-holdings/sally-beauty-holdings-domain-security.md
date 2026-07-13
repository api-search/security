---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sallybeautyholdings.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sallybeauty.com
  spf: true
hosts:
- cert_expires: Jan 31 07:53:06 2027 GMT
  host: www.sallybeautyholdings.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.sallybeauty.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.cosmoprofbeauty.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sally Beauty Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sally Beauty Holdings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sally Beauty Holdings
provider_slug: sally-beauty-holdings
slug: sally-beauty-holdings-domain-security
source_filename: sally-beauty-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sallybeautyholdings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 07:53:06 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.sallybeauty.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n- host: www.cosmoprofbeauty.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sallybeautyholdings.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sallybeauty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sally-beauty-holdings/refs/heads/main/security/sally-beauty-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Beauty
- Retail
- Ecommerce
- Professional
- Consumer
- Fortune 1000
---
