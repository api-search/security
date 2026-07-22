---
api_specs:
- filename: rasgo-openapi.yml
  format: yaml
  label: Rasgo API
  slug: rasgo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasgo/refs/heads/main/openapi/rasgo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: rasgoml.com
  spf: true
hosts:
- host: www.rasgoml.com
  https: false
- cert_expires: Aug 31 06:28:10 2026 GMT
  host: docs.rasgoml.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.rasgoml.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rasgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rasgo, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Rasgo
provider_slug: rasgo
slug: rasgo-domain-security
source_filename: rasgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rasgoml.com\n  https: false\n- host: docs.rasgoml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:28:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rasgoml.com\n  https: false\ndomains:\n- domain: rasgoml.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rasgo/refs/heads/main/security/rasgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Data Warehouse
- Analytics
- Artificial Intelligence
- Natural Language
- Snowflake
- BigQuery
- Business Intelligence
- Metadata
- SQL
---
