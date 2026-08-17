---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: designstripe.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: visual.app
  spf: false
hosts:
- cert_expires: Oct 26 14:52:12 2026 GMT
  host: designstripe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 02:06:07 2026 GMT
  host: visual.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Designstripe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for designstripe, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: designstripe
provider_slug: designstripe
slug: designstripe-domain-security
source_filename: designstripe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: designstripe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 14:52:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: visual.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 02:06:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: designstripe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: visual.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/designstripe/refs/heads/main/security/designstripe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Design
- Artificial Intelligence
- Presentations
- Go-To-Market
- Marketing
- Generative AI
- SaaS
---
