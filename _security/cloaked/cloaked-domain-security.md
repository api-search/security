---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cloaked.com
  spf: true
hosts:
- cert_expires: Sep 13 19:03:31 2026 GMT
  host: www.cloaked.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloaked Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloaked, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cloaked
provider_slug: cloaked
slug: cloaked-domain-security
source_filename: cloaked-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloaked.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:03:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloaked.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloaked/refs/heads/main/security/cloaked-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Privacy
- Identity
- Security
- Data Removal
- Password Manager
- Consumer
- Masked Email
- Virtual Phone
- Identity Theft Protection
---
