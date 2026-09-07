---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 2bytescorp.com
  spf: true
hosts:
- cert_expires: Oct 25 21:53:11 2026 GMT
  host: www.2bytescorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 2Bytes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2bytes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 2bytes
provider_slug: 2bytes
slug: 2bytes-domain-security
source_filename: 2bytes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.2bytescorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 21:53:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 2bytescorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2bytes/refs/heads/main/security/2bytes-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Game Services
- Localization
- Quality Assurance
- Publishing
- HTML5
- South Korea
---
