---
api_specs:
- filename: powerbi.json
  format: json
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/powerbi/data-plane/Microsoft.PowerBI/stable/v1.0/powerbi.json
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: powerbi.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 16 16:30:49 2026 GMT
  host: app.powerbi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 05:54:32 2026 GMT
  host: api.powerbi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Power Bi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Power BI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Power BI
provider_slug: power-bi
slug: power-bi-domain-security
source_filename: power-bi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.powerbi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 16:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.powerbi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 05:54:32 2026 GMT\n  hsts: null\ndomains:\n- domain: powerbi.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power-bi/refs/heads/main/security/power-bi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Analysis
- Reporting
- Visualization
---
