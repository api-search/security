---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: redtri.com
  spf: true
hosts:
- cert_expires: Sep 14 10:22:41 2026 GMT
  host: redtri.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red Tricycle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Tricycle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Red Tricycle
provider_slug: red-tricycle
slug: red-tricycle-domain-security
source_filename: red-tricycle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redtri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:22:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: redtri.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-tricycle/refs/heads/main/security/red-tricycle-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Parenting
- Media
- Family
- Content
- Local
- Lifestyle
- Acquired
---
