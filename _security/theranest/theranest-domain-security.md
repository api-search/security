---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theranest.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ensorahealth.com
  spf: true
hosts:
- cert_expires: Sep 21 21:14:23 2026 GMT
  host: theranest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 21:46:13 2026 GMT
  host: ensorahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Theranest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheraNest, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TheraNest
provider_slug: theranest
slug: theranest-domain-security
source_filename: theranest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theranest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:14:23 2026 GMT\n  hsts: false\n- host: ensorahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:46:13 2026 GMT\n  hsts: false\ndomains:\n- domain: theranest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ensorahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theranest/refs/heads/main/security/theranest-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Behavioral Health
- Mental Health
- EHR
- Practice Management
- Healthcare
- HIPAA
- Telehealth
- Ensora Health
- Therapy Brands
---
