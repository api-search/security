---
api_specs:
- filename: algodriven-vehicle-history-openapi.yml
  format: yaml
  label: Vehicle History Report - UAE
  slug: vehicle-history-report-uae
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algodriven/refs/heads/main/openapi/algodriven-vehicle-history-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: algodriven.xyz
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: algodriven.io
  spf: false
hosts:
- cert_expires: Sep 29 05:50:40 2026 GMT
  host: algodriven.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: algodriven.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Algodriven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlgoDriven, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AlgoDriven
provider_slug: algodriven
slug: algodriven-domain-security
source_filename: algodriven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: algodriven.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:50:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: algodriven.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: algodriven.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: algodriven.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algodriven/refs/heads/main/security/algodriven-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Vehicle Data
- Car Valuation
- Vehicle Inspection
- Artificial Intelligence
- Vehicle History
- Automotive Data Intelligence
---
