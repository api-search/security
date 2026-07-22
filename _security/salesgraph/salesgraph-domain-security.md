---
api_specs:
- filename: salesgraph-openapi.yml
  format: yaml
  label: Salesgraph REST API
  slug: salesgraph-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/openapi/salesgraph-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: salesgraph.com
  spf: true
hosts:
- cert_expires: Aug 25 04:55:49 2026 GMT
  host: docs.salesgraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:54:39 2026 GMT
  host: salesgraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salesgraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesgraph, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Salesgraph
provider_slug: salesgraph
slug: salesgraph-domain-security
source_filename: salesgraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.salesgraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 04:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: salesgraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:54:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: salesgraph.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesgraph/refs/heads/main/security/salesgraph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales
- Revenue Automation
- Go-To-Market
- AI Agents
- MCP
- Sales Intelligence
- Competitive Intelligence
- Research
- Enterprise Sales
---
