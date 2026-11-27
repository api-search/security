---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: comontel.fr
  spf: true
hosts:
- cert_expires: Jan  3 20:13:32 2027 GMT
  host: comontel.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Comontel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comontel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Comontel
provider_slug: comontel-fr
slug: comontel-fr-domain-security
source_filename: comontel-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comontel.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 20:13:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: comontel.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/comontel-fr/security/comontel-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Telecommunications
- Mobile
- MVNO
- Cross-Border
- France
- Switzerland
- Small Business
- MCP
---
