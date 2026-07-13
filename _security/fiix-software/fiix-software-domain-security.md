---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fiixsoftware.com
  spf: true
hosts:
- cert_expires: Sep 13 07:28:41 2026 GMT
  host: fiixsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.fiixsoftware.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fiix Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fiix Software, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fiix Software
provider_slug: fiix-software
slug: fiix-software-domain-security
source_filename: fiix-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fiixsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:28:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fiixsoftware.com\n  https: false\ndomains:\n- domain: fiixsoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiix-software/refs/heads/main/security/fiix-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMMS
- Maintenance Management
- Asset Management
- Manufacturing
- Reliability
- Work Orders
---
