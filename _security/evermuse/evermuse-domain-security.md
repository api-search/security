---
api_specs:
- filename: evermuse-ingest-v1-openapi-original.yml
  format: yaml
  label: Evermuse Ingestion API
  slug: evermuse-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evermuse/refs/heads/main/openapi/evermuse-ingest-v1-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: evermuse.com
  spf: true
hosts:
- cert_expires: Sep 27 21:39:25 2026 GMT
  host: evermuse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 06:59:42 2026 GMT
  host: api.evermuse.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evermuse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evermuse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Evermuse
provider_slug: evermuse
slug: evermuse-domain-security
source_filename: evermuse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evermuse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:39:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.evermuse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 06:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: evermuse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evermuse/refs/heads/main/security/evermuse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Product Management
- Customer Feedback
- Voice of Customer
- Artificial Intelligence
- Data Ingestion
- Product Analytics
- MCP
- Developer Tools
---
