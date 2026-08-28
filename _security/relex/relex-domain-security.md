---
api_specs:
- filename: relex-data-api-openapi.json
  format: json
  label: RELEX Data API
  slug: relex-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/openapi/relex-data-api-openapi.json
- filename: relex-monitoring-api-openapi.json
  format: json
  label: RELEX Monitoring API
  slug: relex-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/openapi/relex-monitoring-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: relexsolutions.com
  spf: true
hosts:
- cert_expires: Nov  6 08:18:00 2026 GMT
  host: www.relexsolutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 16:32:36 2026 GMT
  host: eu.rest.relexsolutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 20:53:47 2026 GMT
  host: eu.monitor.relexsolutions.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RELEX Solutions, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RELEX Solutions
provider_slug: relex
slug: relex-domain-security
source_filename: relex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.relexsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 08:18:00 2026 GMT\n  hsts: false\n- host: eu.rest.relexsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 16:32:36 2026 GMT\n  hsts: null\n- host: eu.monitor.relexsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:53:47 2026 GMT\n  hsts: null\ndomains:\n- domain: relexsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relex/refs/heads/main/security/relex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Supply Chain
- Retail
- Demand Planning
- Inventory Management
- Forecasting
- Pricing
- Enterprise Software
- Data Integration
- Company
---
