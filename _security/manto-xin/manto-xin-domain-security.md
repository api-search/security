---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: manto.xin
  spf: false
hosts:
- cert_expires: Dec  1 01:40:07 2026 GMT
  host: manto.xin
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Manto News Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manto News, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Manto News
provider_slug: manto-xin
slug: manto-xin-domain-security
source_filename: manto-xin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manto.xin\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 01:40:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: manto.xin\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/manto-xin/security/manto-xin-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- News
- RSS
- MCP
---
