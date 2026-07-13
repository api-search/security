---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tjx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mytjx.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.tjx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: www.mytjx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 23 20:56:55 2026 GMT
  host: www.spscommerce.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tjx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TJX Companies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TJX Companies
provider_slug: tjx
slug: tjx-domain-security
source_filename: tjx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tjx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\n- host: www.mytjx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: false\n- host: www.spscommerce.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 23 20:56:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: tjx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mytjx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tjx/refs/heads/main/security/tjx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Off-Price
- Fortune 100
- Supply Chain
- EDI
---
