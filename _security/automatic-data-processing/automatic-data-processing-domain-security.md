---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adp.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: developers.adp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.adp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: api.adp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Automatic Data Processing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automatic Data Processing (ADP), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Automatic Data Processing (ADP)
provider_slug: automatic-data-processing
slug: automatic-data-processing-domain-security
source_filename: automatic-data-processing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.adp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.adp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\n- host: api.adp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automatic-data-processing/refs/heads/main/security/automatic-data-processing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HCM
- Human Capital Management
- HR
- Payroll
- Benefits
- Workforce Management
- Tax Compliance
- Enterprise
- Fortune 500
---
