---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: playbackbone.com
  spf: true
hosts:
- cert_expires: Aug 22 19:09:00 2026 GMT
  host: playbackbone.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Backbone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backbone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Backbone
provider_slug: backbone
slug: backbone-domain-security
source_filename: backbone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playbackbone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 19:09:00 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: playbackbone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backbone/refs/heads/main/security/backbone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Entertainment
- Gaming
- Mobile Gaming
- Gaming Controller
- Consumer Electronics
- Hardware
- Ecommerce
---
