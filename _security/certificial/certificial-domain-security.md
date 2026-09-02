---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: certificial.com
  spf: true
hosts:
- cert_expires: Sep 28 12:14:34 2026 GMT
  host: www.certificial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: my.certificial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Certificial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certificial, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Certificial
provider_slug: certificial
slug: certificial-domain-security
source_filename: certificial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.certificial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:14:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.certificial.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: certificial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certificial/refs/heads/main/security/certificial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Certificate of Insurance
- Risk Management
- Compliance
- Supplier Management
- Insurance Verification
- ACORD
- Company
---
