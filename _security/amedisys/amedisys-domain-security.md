---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amedisys.com
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.amedisys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.amedisys.com
  https: false
- host: api.amedisys.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amedisys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amedisys, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amedisys
provider_slug: amedisys
slug: amedisys-domain-security
source_filename: amedisys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amedisys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.amedisys.com\n  https: false\n- host: api.amedisys.com\n  https: false\ndomains:\n- domain: amedisys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amedisys/refs/heads/main/security/amedisys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Home Health
- Hospice
- Healthcare
---
