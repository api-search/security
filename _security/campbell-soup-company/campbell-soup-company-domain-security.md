---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thecampbellscompany.com
  spf: true
hosts:
- cert_expires: Oct  1 01:01:50 2026 GMT
  host: www.thecampbellscompany.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 15:30:57 2026 GMT
  host: investor.thecampbellscompany.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: careers.thecampbellscompany.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Campbell Soup Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Campbell''s Company, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Campbell's Company
provider_slug: campbell-soup-company
slug: campbell-soup-company-domain-security
source_filename: campbell-soup-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thecampbellscompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:01:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: investor.thecampbellscompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:30:57 2026 GMT\n  hsts: null\n- host: careers.thecampbellscompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thecampbellscompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campbell-soup-company/refs/heads/main/security/campbell-soup-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Beverages
- Consumer Packaged Goods
- CPG
- Food
- Meals
- Snacks
- Soup
- Fortune 500
---
