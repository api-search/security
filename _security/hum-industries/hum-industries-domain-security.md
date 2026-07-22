---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: humindustries.com
  spf: false
hosts:
- cert_expires: Sep 11 15:14:39 2026 GMT
  host: humindustries.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hum Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HUM Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HUM Industries
provider_slug: hum-industries
slug: hum-industries-domain-security
source_filename: hum-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humindustries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:14:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humindustries.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hum-industries/refs/heads/main/security/hum-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Wearables
- Artificial Intelligence
- Consumer Hardware
- Voice
- Memory
- AI Assistant
---
