---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cority.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: enviance.com
  spf: true
hosts:
- cert_expires: Sep  8 17:38:49 2026 GMT
  host: cority.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.enviance.com
  hsts: true
  hsts_max_age: 900
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cority Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cority, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cority
provider_slug: cority
slug: cority-domain-security
source_filename: cority-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cority.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:38:49 2026 GMT\n  hsts: false\n- host: api.enviance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 900\ndomains:\n- domain: cority.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: enviance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cority/refs/heads/main/security/cority-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Environmental Health and Safety
- EHS
- Sustainability
- ESG
- Occupational Health
- Quality Management
- Compliance
- Enterprise Software
---
