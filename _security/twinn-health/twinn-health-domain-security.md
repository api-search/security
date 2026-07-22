---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: twinn.health
  spf: true
hosts:
- cert_expires: Sep 21 13:59:19 2026 GMT
  host: twinn.health
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twinn Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twinn Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Twinn Health
provider_slug: twinn-health
slug: twinn-health-domain-security
source_filename: twinn-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: twinn.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 13:59:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: twinn.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twinn-health/refs/heads/main/security/twinn-health-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Medical Imaging
- MRI
- Preventive Health
- Artificial Intelligence
- Diagnostics
- Longevity
---
