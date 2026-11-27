---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: compera.se
  spf: true
hosts:
- cert_expires: Jan 28 04:05:48 2027 GMT
  host: compera.se
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Compera
provider_slug: compera-se
slug: compera-se-domain-security
source_filename: compera-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compera.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 04:05:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: compera.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/compera-se/security/compera-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Price Comparison
- Sweden
- Consumer Finance
- Insurance
- Electricity
- Broadband
- MCP
---
