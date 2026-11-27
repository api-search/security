---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: occam.fit
  spf: false
hosts:
- cert_expires: Dec 27 17:34:19 2026 GMT
  host: occam.fit
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Occam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Occam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Occam
provider_slug: occam-fit
slug: occam-fit-domain-security
source_filename: occam-fit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: occam.fit\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 17:34:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: occam.fit\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/occam-fit/security/occam-fit-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Machine Learning
- Symbolic Regression
- Data Analysis
- MCP Server
- Open Source
---
