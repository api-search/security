---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: runlaminar.com
  spf: true
hosts:
- cert_expires: Dec 14 21:59:04 2026 GMT
  host: runlaminar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Runlaminar Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laminar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Laminar
provider_slug: runlaminar-com
slug: runlaminar-com-domain-security
source_filename: runlaminar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runlaminar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 21:59:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: runlaminar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/runlaminar-com/security/runlaminar-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sensors
- AI
- Manufacturing
- FoodTech
- CPG
---
