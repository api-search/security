---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rightwayhealthcare.com
  spf: true
hosts:
- cert_expires: Sep  1 11:46:02 2026 GMT
  host: www.rightwayhealthcare.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: member.rightwayhealthcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:37:56 2026 GMT
  host: api.rightwayhealthcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rightway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rightway, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rightway
provider_slug: rightway
slug: rightway-domain-security
source_filename: rightway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rightwayhealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:46:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: member.rightwayhealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n- host: api.rightwayhealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:37:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rightwayhealthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightway/refs/heads/main/security/rightway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Pharmacy Benefits
- PBM
- Care Navigation
- Health Insurance
- Employee Benefits
- Digital Health
- HIPAA
---
