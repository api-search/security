---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aecom.com
  spf: true
hosts:
- cert_expires: Sep 26 19:55:59 2026 GMT
  host: www.aecom.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: digital.aecom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 20:19:13 2026 GMT
  host: investors.aecom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aecom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AECOM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AECOM
provider_slug: aecom
slug: aecom-domain-security
source_filename: aecom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aecom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:55:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: digital.aecom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: investors.aecom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:19:13 2026 GMT\n  hsts: null\ndomains:\n- domain: aecom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aecom/refs/heads/main/security/aecom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Engineering
- Infrastructure
- Construction
- Environmental Services
- Transportation
- Fortune 500
---
