---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: hoibi.de
  spf: false
hosts:
- cert_expires: Dec 22 13:50:24 2026 GMT
  host: hoibi.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hoibi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hoibi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Hoibi
provider_slug: hoibi-de
slug: hoibi-de-domain-security
source_filename: hoibi-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hoibi.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 13:50:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hoibi.de\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hoibi-de/security/hoibi-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Affiliates
- SEO
- Content
- Marketing
- Geo
---
