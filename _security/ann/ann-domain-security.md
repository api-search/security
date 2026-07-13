---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anntaylor.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: loft.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.anntaylor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.loft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.knitwellgroup.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ann Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ANN Inc., probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ANN Inc.
provider_slug: ann
slug: ann-domain-security
source_filename: ann-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anntaylor.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.loft.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.knitwellgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: anntaylor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: loft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ann/refs/heads/main/security/ann-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Ann Taylor
- Fashion
- KnitWell
- LOFT
- Lou And Grey
- Retail
- Sycamore Partners
- Women's Apparel
---
