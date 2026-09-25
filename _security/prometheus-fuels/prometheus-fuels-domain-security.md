---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prometheusfuels.ai
  spf: false
hosts:
- cert_expires: Oct 24 11:46:56 2026 GMT
  host: prometheusfuels.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prometheus Fuels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prometheus Fuels, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Prometheus Fuels
provider_slug: prometheus-fuels
slug: prometheus-fuels-domain-security
source_filename: prometheus-fuels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prometheusfuels.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 11:46:56 2026 GMT\n  hsts: null\ndomains:\n- domain: prometheusfuels.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prometheus-fuels/refs/heads/main/security/prometheus-fuels-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Energy
- Climate Tech
- Carbon Capture
- Synthetic Fuels
- Direct Air Capture
- Energy Storage
- content-api
- WordPress
---
