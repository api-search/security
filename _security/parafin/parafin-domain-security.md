---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parafin.com
  spf: true
hosts:
- cert_expires: Sep 10 22:11:38 2026 GMT
  host: www.parafin.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 06:02:49 2026 GMT
  host: docs.parafin.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.parafin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parafin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parafin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parafin
provider_slug: parafin
slug: parafin-domain-security
source_filename: parafin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parafin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:11:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.parafin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 06:02:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.parafin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parafin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parafin/refs/heads/main/security/parafin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Embedded Finance
- Lending
- Capital
- Payments
- Small Business
- Working Capital
- API
---
