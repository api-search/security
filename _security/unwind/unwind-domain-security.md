---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: unwind.me
  spf: false
hosts:
- cert_expires: Nov 16 13:52:30 2026 GMT
  host: unwind.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unwind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unwind Me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Unwind Me
provider_slug: unwind
slug: unwind-domain-security
source_filename: unwind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unwind.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 13:52:30 2026 GMT\n  hsts: false\ndomains:\n- domain: unwind.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unwind/refs/heads/main/security/unwind-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Massage
- Wellness
- On-Demand Services
- Consumer
- Marketplace
- Defunct
- Acquired
---
