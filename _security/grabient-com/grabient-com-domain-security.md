---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grabient.com
  spf: true
hosts:
- cert_expires: Jan 16 18:32:48 2027 GMT
  host: grabient.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grabient Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grabient, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Grabient
provider_slug: grabient-com
slug: grabient-com-domain-security
source_filename: grabient-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grabient.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 18:32:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grabient.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/grabient-com/security/grabient-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CSS
- Gradient
- Design
- Color
- Palette
---
