---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tassvision.ai
  spf: true
hosts:
- cert_expires: Aug 30 06:26:05 2026 GMT
  host: tassvision.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tass Vision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tass Vision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tass Vision
provider_slug: tass-vision
slug: tass-vision-domain-security
source_filename: tass-vision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tassvision.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:26:05 2026 GMT\n  hsts: false\ndomains:\n- domain: tassvision.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tass-vision/refs/heads/main/security/tass-vision-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Startup
- Venture Backed
- 500 Global
- SITRAC
- VITRAC
---
