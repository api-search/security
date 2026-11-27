---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: insiderkauf.de
  spf: true
hosts:
- cert_expires: Jan 10 22:19:28 2027 GMT
  host: insiderkauf.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Insiderkauf.de Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insiderkauf.de, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Insiderkauf.de
provider_slug: insiderkauf-de
slug: insiderkauf-de-domain-security
source_filename: insiderkauf-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insiderkauf.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 22:19:28 2027 GMT\n  hsts: false\ndomains:\n- domain: insiderkauf.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://artifacts.apis.io/insiderkauf-de/security/insiderkauf-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Stock Market
- Insider Trading
- Germany
- Data
---
