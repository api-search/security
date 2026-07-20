---
description: ''
domains:
- caa:
  - 0 issue "cybertrust.ne.jp"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issue "quovadisglobal.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cegid.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cegid.be
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.cegid.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 08:49:12 2026 GMT
  host: developers.cegid.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: connect.koalaboox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Koalaboox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Koalaboox, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Koalaboox
provider_slug: koalaboox
slug: koalaboox-domain-security
source_filename: koalaboox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cegid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.cegid.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:49:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.koalaboox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cegid.com\n  dnssec: false\n  caa:\n  - 0 issue \"cybertrust.ne.jp\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"quovadisglobal.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cegid.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koalaboox/refs/heads/main/security/koalaboox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Invoicing
- Electronic Invoicing
- Peppol
- Accounting
- Invoice Financing
- Working Capital
- Small Business
- Fintech
- Belgium
- Spain
- OAuth
---
