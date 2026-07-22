---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nlyte.com
  spf: true
hosts:
- cert_expires: Aug 30 03:38:40 2026 GMT
  host: www.nlyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nlyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nlyte, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: nlyte
provider_slug: nlyte
slug: nlyte-domain-security
source_filename: nlyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nlyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:38:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nlyte.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nlyte/refs/heads/main/security/nlyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Center
- DCIM
- Infrastructure Management
- Asset Management
- IT Operations
- Connectors
- REST API
---
