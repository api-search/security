---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 5nine.com
  spf: true
hosts:
- cert_expires: Oct  6 06:17:23 2026 GMT
  host: 5nine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: 5Nine Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 5Nine Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 5Nine Software
provider_slug: 5nine-software
slug: 5nine-software-domain-security
source_filename: 5nine-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 5nine.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 06:17:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 5nine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/5nine-software/refs/heads/main/security/5nine-software-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Hyper-V
- Cloud Management
- Microsoft Azure
- Managed Service Providers
- Acquired
---
