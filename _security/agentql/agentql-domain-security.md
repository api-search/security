---
api_specs:
- filename: agentql-openapi.yaml
  format: yaml
  label: AgentQL Query Data API
  slug: query-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/openapi/agentql-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: agentql.com
  spf: true
hosts:
- cert_expires: Sep 28 17:26:44 2026 GMT
  host: www.agentql.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 05:26:59 2026 GMT
  host: docs.agentql.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.agentql.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agentql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgentQL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AgentQL
provider_slug: agentql
slug: agentql-domain-security
source_filename: agentql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agentql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:26:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.agentql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:26:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.agentql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: agentql.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/security/agentql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
---
