---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: americanwoodmark.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: woodmark.com
  spf: true
hosts:
- cert_expires: Feb  3 16:42:27 2027 GMT
  host: www.americanwoodmark.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 19:23:27 2027 GMT
  host: id.woodmark.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Woodmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Woodmark, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: American Woodmark
provider_slug: american-woodmark
slug: american-woodmark-domain-security
source_filename: american-woodmark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.americanwoodmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 16:42:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: id.woodmark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 19:23:27 2027 GMT\n  hsts: null\ndomains:\n- domain: americanwoodmark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: woodmark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-woodmark/refs/heads/main/security/american-woodmark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cabinetry
- Home Products
- Construction
- Building Products
- Manufacturing
- Kitchen and Bath
- Home Improvement
- Identity
- EDI
- Supply Chain
---
