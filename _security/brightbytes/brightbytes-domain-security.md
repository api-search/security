---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightbytes.net
  spf: true
hosts:
- cert_expires: Oct 14 04:49:20 2026 GMT
  host: www.brightbytes.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightbytes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrightBytes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BrightBytes
provider_slug: brightbytes
slug: brightbytes-domain-security
source_filename: brightbytes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightbytes.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 04:49:20 2026 GMT\n  hsts: null\ndomains:\n- domain: brightbytes.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightbytes/refs/heads/main/security/brightbytes-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Education
- Analytics
- Data
- K-12
- EdTech
- Acquired
---
