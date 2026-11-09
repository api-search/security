---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boonful.io
  spf: true
hosts:
- cert_expires: Dec 12 06:59:30 2026 GMT
  host: boonful.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boonful Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boonful, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Boonful
provider_slug: boonful-io
slug: boonful-io-domain-security
source_filename: boonful-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boonful.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 06:59:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boonful.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/boonful-io/security/boonful-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Publishing
- Software-as-a-Service
- E-Commerce
- Content Creation
- No-Code
---
