---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: valspar.com
  spf: true
- caa:
  - 0 issue "awstrust.com"
  - 128 issue "entrust.net"
  - 128 issue "digicert.com"
  - 128 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sherwin-williams.com
  spf: true
hosts:
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: www.valspar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.sherwin-williams.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valspar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valspar, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Valspar
provider_slug: valspar
slug: valspar-domain-security
source_filename: valspar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.valspar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.sherwin-williams.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: valspar.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sherwin-williams.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 128 issue \"entrust.net\"\n  - 128 issue \"digicert.com\"\n  - 128 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valspar/refs/heads/main/security/valspar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Paint
- Coatings
- Manufacturing
- Consumer Goods
- Fortune 1000
---
