---
api_specs:
- filename: airbyte-openapi.yml
  format: yaml
  label: Airbyte
  slug: airbyte
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/openapi/airbyte-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: airbyte.com
  spf: true
hosts:
- cert_expires: Aug 26 02:42:56 2026 GMT
  host: airbyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 16:27:13 2026 GMT
  host: api.airbyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airbyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airbyte, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Airbyte
provider_slug: airbyte
slug: airbyte-domain-security
source_filename: airbyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airbyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:42:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.airbyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:27:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airbyte.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/security/airbyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
---
