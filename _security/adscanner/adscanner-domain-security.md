---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alleyesonscreens.com
  spf: true
hosts:
- cert_expires: Oct 14 21:35:37 2026 GMT
  host: www.alleyesonscreens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adscanner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adscanner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adscanner
provider_slug: adscanner
slug: adscanner-domain-security
source_filename: adscanner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alleyesonscreens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:35:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alleyesonscreens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adscanner/refs/heads/main/security/adscanner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Television
- Media Measurement
- Analytics
- Attribution
- Connected TV
- Addressable TV
- Audience Data
- Artificial Intelligence
- Croatia
---
