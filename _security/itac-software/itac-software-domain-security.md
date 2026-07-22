---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: itacsoftware.com
  spf: true
hosts:
- cert_expires: Aug  3 07:08:40 2026 GMT
  host: www.itacsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itac Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iTAC Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iTAC Software
provider_slug: itac-software
slug: itac-software-domain-security
source_filename: itac-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.itacsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 07:08:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: itacsoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itac-software/refs/heads/main/security/itac-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- Manufacturing
- MES
- MOM
- Industry 4.0
- Smart Factory
- IoT
- Automotive
- Electronics
- Traceability
---
