---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lexyomlaw.com
  spf: false
hosts:
- cert_expires: Sep 26 05:31:22 2026 GMT
  host: lexyomlaw.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lexyom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lexyom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lexyom
provider_slug: lexyom
slug: lexyom-domain-security
source_filename: lexyom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lexyomlaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lexyomlaw.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexyom/refs/heads/main/security/lexyom-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Legal
- Legal Services
- Law Firm
- Financial Services
- Regulatory Compliance
- Licensing
- Trademarks
- Intellectual Property
- Corporate Services
- MENA
---
