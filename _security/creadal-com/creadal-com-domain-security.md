---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: creadal.com
  spf: true
hosts:
- cert_expires: Jan  7 22:49:00 2027 GMT
  host: creadal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Creadal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creadal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Creadal
provider_slug: creadal-com
slug: creadal-com-domain-security
source_filename: creadal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creadal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 22:49:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: creadal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/creadal-com/security/creadal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Design
- Templates
- Packaging
- Mockups
- Dielines
- MCP
- Graphic Design
---
