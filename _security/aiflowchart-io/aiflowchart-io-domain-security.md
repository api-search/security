---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aiflowchart.io
  spf: true
hosts:
- cert_expires: Jan 19 08:34:15 2027 GMT
  host: aiflowchart.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiflowchart Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Flowchart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Flowchart
provider_slug: aiflowchart-io
slug: aiflowchart-io-domain-security
source_filename: aiflowchart-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiflowchart.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 08:34:15 2027 GMT\n  hsts: false\ndomains:\n- domain: aiflowchart.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aiflowchart-io/security/aiflowchart-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Diagram
- Flowchart
- Generator
- Free
---
