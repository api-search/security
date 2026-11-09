---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: findmetry.com
  spf: true
hosts:
- cert_expires: Dec 15 11:39:26 2026 GMT
  host: findmetry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Findmetry Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Findmetry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Findmetry
provider_slug: findmetry-com
slug: findmetry-com-domain-security
source_filename: findmetry-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findmetry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 11:39:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: findmetry.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/findmetry-com/security/findmetry-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Website
- Diagnostics
- Evidence
- Technical
- Service
---
