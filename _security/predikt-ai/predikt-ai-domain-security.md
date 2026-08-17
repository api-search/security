---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: predikdata.com
  spf: true
hosts:
- cert_expires: Nov  8 02:57:43 2026 GMT
  host: predikdata.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api.predikdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Predikt Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PREDIK Data-Driven, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PREDIK Data-Driven
provider_slug: predikt-ai
slug: predikt-ai-domain-security
source_filename: predikt-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: predikdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 02:57:43 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.predikdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: predikdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predikt-ai/refs/heads/main/security/predikt-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Intelligence
- Data Enrichment
- Company Data
- B2B Data
- Sales Intelligence
- Reference Data
- Location Intelligence
- Geospatial
- Foot Traffic
- POI Data
- Mobility Data
- Demand Forecasting
- Site Selection
- Alternative Data
---
