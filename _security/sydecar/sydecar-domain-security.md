---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sydecar.io
  spf: true
hosts:
- cert_expires: Aug 27 16:38:21 2026 GMT
  host: sydecar.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 13:53:48 2026 GMT
  host: api-docs.sydecar.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 06:33:19 2026 GMT
  host: api.sydecar.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sydecar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sydecar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sydecar
provider_slug: sydecar
slug: sydecar-domain-security
source_filename: sydecar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sydecar.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:38:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.sydecar.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:53:48 2026 GMT\n  hsts: null\n- host: api.sydecar.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 06:33:19 2026 GMT\n  hsts: null\ndomains:\n- domain: sydecar.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sydecar/refs/heads/main/security/sydecar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Fintech
- Venture Capital
- SPV
- Investment
- Compliance
- API
---
