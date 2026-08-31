---
api_specs:
- filename: databook-batch-create-api-openapi.yml
  format: yaml
  label: Databook batch - create API
  slug: databook-batch-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-batch-create-api-openapi.yml
- filename: databook-batch-query-api-openapi.yml
  format: yaml
  label: Databook batch - query API
  slug: databook-batch-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-batch-query-api-openapi.yml
- filename: databook-chat-api-openapi.yml
  format: yaml
  label: Databook Chat API
  slug: databook-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-chat-api-openapi.yml
- filename: databook-reasoning-api-openapi.yml
  format: yaml
  label: Databook Reasoning API
  slug: databook-reasoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/openapi/databook-reasoning-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: databook.com
  spf: true
hosts:
- cert_expires: Oct 15 21:39:46 2026 GMT
  host: databook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: api.databook.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Databook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Databook, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Databook
provider_slug: databook
slug: databook-domain-security
source_filename: databook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: databook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.databook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: databook.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databook/refs/heads/main/security/databook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Vertical Software
- Sales Intelligence
- Account Intelligence
- Sales Enablement
- Enterprise Sales
- Artificial Intelligence
- Revenue Operations
- REST API
- OpenAPI
- Batch Processing
- Agents
- Reasoning
- Company Data
---
