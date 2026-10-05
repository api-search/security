---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: safe.com
  spf: true
hosts:
- cert_expires: Dec 22 06:29:30 2026 GMT
  host: www.safe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Safe Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safe Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Safe Software
provider_slug: safe-software
slug: safe-software-domain-security
source_filename: safe-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.safe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 06:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: safe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safe-software/refs/heads/main/security/safe-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Integration
- Spatial Analytics
- Artificial Intelligence
- Enterprise
---
