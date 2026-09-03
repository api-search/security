---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: code24.nl
  spf: true
hosts:
- cert_expires: Oct 12 13:47:50 2026 GMT
  host: www.code24.nl
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Code24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Code24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Code24
provider_slug: code24
slug: code24-domain-security
source_filename: code24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.code24.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 13:47:50 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: code24.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code24/refs/heads/main/security/code24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Electronic Health Records
- openEHR
- FHIR
- MedMij
- Interoperability
- Mental Health
- Netherlands
- Health Data
---
