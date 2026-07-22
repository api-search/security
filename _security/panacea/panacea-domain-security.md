---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: withpanacea.com
  spf: false
hosts:
- cert_expires: Oct 14 13:40:40 2026 GMT
  host: withpanacea.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Panacea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panacea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Panacea
provider_slug: panacea
slug: panacea-domain-security
source_filename: panacea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withpanacea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 13:40:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: withpanacea.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panacea/refs/heads/main/security/panacea-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Regulatory
- FDA
- Healthcare
- Life Sciences
- Medical Devices
- Pharmaceuticals
- Consulting
- Artificial Intelligence
---
