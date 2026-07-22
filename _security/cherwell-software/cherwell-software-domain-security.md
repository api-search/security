---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cherwell.com
  spf: true
hosts:
- cert_expires: Sep 13 03:34:37 2026 GMT
  host: www.cherwell.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cherwell Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cherwell Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cherwell Software
provider_slug: cherwell-software
slug: cherwell-software-domain-security
source_filename: cherwell-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cherwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:34:37 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: cherwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cherwell-software/refs/heads/main/security/cherwell-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IT Service Management
- ITSM
- Enterprise Service Management
- IT Asset Management
- ITAM
- Acquired
- Ivanti
---
