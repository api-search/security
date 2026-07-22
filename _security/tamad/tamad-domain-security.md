---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flowly.world
  spf: true
hosts:
- cert_expires: Oct 16 08:19:03 2026 GMT
  host: flowly.world
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tamad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tamadé, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tamadé
provider_slug: tamad
slug: tamad-domain-security
source_filename: tamad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowly.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 08:19:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowly.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tamad/refs/heads/main/security/tamad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Telehealth
- Digital Health
- Chronic Pain
- Mental Health
- Consumer
---
