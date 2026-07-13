---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: payoneer.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.payoneer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.payoneer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: checkoutdocs.payoneer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payoneer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payoneer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Payoneer
provider_slug: payoneer
slug: payoneer-domain-security
source_filename: payoneer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.payoneer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.payoneer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n- host: checkoutdocs.payoneer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: payoneer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payoneer/refs/heads/main/security/payoneer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- payments
- payouts
- cross-border payments
- currency conversion
- marketplace payments
- fintech
- financial services
- mass payouts
- checkout
- REST
---
