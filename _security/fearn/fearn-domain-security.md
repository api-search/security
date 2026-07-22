---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fearn.ai
  spf: true
hosts:
- cert_expires: Sep  8 10:09:48 2026 GMT
  host: fearn.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fearn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fearn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fearn
provider_slug: fearn
slug: fearn-domain-security
source_filename: fearn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fearn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:09:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fearn.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fearn/refs/heads/main/security/fearn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Patents
- Intellectual Property
- Legal Tech
- Patent Prosecution
- Artificial Intelligence
- Legal Services
- Startups
---
