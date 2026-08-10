---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arraybc.com
  spf: true
hosts:
- cert_expires: Sep 13 20:50:41 2026 GMT
  host: arraybc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Array Behavioral Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Array Behavioral Care, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Array Behavioral Care
provider_slug: array-behavioral-care
slug: array-behavioral-care-domain-security
source_filename: array-behavioral-care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arraybc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 20:50:41 2026 GMT\n  hsts: false\ndomains:\n- domain: arraybc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/array-behavioral-care/refs/heads/main/security/array-behavioral-care-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Behavioral Health
- Mental Health
- Telehealth
- Telepsychiatry
- Digital Health
- Electronic Health Records
- Patient Engagement
- HIPAA
---
