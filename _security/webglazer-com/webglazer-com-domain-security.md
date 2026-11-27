---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: webglazer.com
  spf: true
hosts:
- cert_expires: Feb  8 08:13:15 2027 GMT
  host: webglazer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: WebGlazer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WebGlazer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: WebGlazer
provider_slug: webglazer-com
slug: webglazer-com-domain-security
source_filename: webglazer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: webglazer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 08:13:15 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: webglazer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/webglazer-com/security/webglazer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Brand Monitoring
- AI Visibility
- Brands
- Agencies
- AI Search
- Dashboards
---
