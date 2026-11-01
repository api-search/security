---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: saka.run
  spf: true
hosts:
- cert_expires: Jan  9 20:59:02 2027 GMT
  host: saka.run
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saka Run Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for saka-run, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: saka-run
provider_slug: saka-run
slug: saka-run-domain-security
source_filename: saka-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saka.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 20:59:02 2027 GMT\n  hsts: false\ndomains:\n- domain: saka.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/saka-run/security/saka-run-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data
- Prospecting
- Marketing
- SaaS
---
