---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: numeric.io
  spf: true
hosts:
- cert_expires: Oct 14 06:35:41 2026 GMT
  host: www.numeric.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 21:53:10 2026 GMT
  host: api.numeric.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Numeric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numeric, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Numeric
provider_slug: numeric
slug: numeric-domain-security
source_filename: numeric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.numeric.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:35:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.numeric.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 21:53:10 2026 GMT\n  hsts: null\ndomains:\n- domain: numeric.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numeric/refs/heads/main/security/numeric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Accounting
- Financial Close
- Reconciliation
- MCP
- Agent Skills
- OAuth
---
