---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: beyond.wine
  spf: false
hosts:
- cert_expires: Jan 26 18:04:41 2027 GMT
  host: beyond.wine
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beyond Wine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beyond Wine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Beyond Wine
provider_slug: beyond-wine
slug: beyond-wine-domain-security
source_filename: beyond-wine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beyond.wine\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 18:04:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beyond.wine\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/beyond-wine/security/beyond-wine-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Beverages
- Non-Alcoholic
- Specialty Drinks
- Knowledge Base
---
