---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carbonridge.com
  spf: false
hosts:
- cert_expires: Nov 26 14:17:11 2026 GMT
  host: www.carbonridge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carbon Ridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbon Ridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Carbon Ridge
provider_slug: carbon-ridge
slug: carbon-ridge-domain-security
source_filename: carbon-ridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carbonridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 14:17:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carbonridge.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbon-ridge/refs/heads/main/security/carbon-ridge-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Maritime
- Carbon Capture
- Sustainability
- CleanTech
---
