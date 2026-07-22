---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: morphsys.ai
  spf: false
hosts:
- cert_expires: Sep 19 07:30:03 2026 GMT
  host: morphsys.ai
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morph Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morph Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Morph Systems
provider_slug: morph-systems
slug: morph-systems-domain-security
source_filename: morph-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morphsys.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:30:03 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\ndomains:\n- domain: morphsys.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morph-systems/refs/heads/main/security/morph-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Consulting
- Palantir
- Large Language Models
- Data
- Supply Chain
- Aerospace and Defense
---
