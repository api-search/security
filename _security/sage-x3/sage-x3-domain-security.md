---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sage.com
  spf: true
hosts:
- cert_expires: Aug 10 23:59:59 2026 GMT
  host: www.sage.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:04:19 2026 GMT
  host: developer.sage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sage X3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sage X3, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sage X3
provider_slug: sage-x3
slug: sage-x3-domain-security
source_filename: sage-x3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.sage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:04:19 2026 GMT\n  hsts: null\ndomains:\n- domain: sage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sage-x3/refs/heads/main/security/sage-x3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Enterprise Resource Planning
- Manufacturing
- Distribution
- Supply Chain
- Financials
- Accounting
- Inventory
- Mid-Market
- Enterprise
---
