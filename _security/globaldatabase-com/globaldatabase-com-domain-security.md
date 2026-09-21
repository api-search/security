---
api_specs:
- filename: globaldatabase-com-mcp-playground-openapi.yml
  format: yaml
  label: Global Database MCP Server
  slug: global-database-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/openapi/globaldatabase-com-mcp-playground-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: globaldatabase.com
  spf: true
hosts:
- cert_expires: Nov 17 22:00:16 2026 GMT
  host: globaldatabase.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Globaldatabase Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Global Database, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Global Database
provider_slug: globaldatabase-com
slug: globaldatabase-com-domain-security
source_filename: globaldatabase-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: globaldatabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 22:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: globaldatabase.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globaldatabase-com/refs/heads/main/security/globaldatabase-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Company Data
- KYB
- Compliance
- Business Verification
- Beneficial Ownership
- Financial
- Credit Risk
- Data Enrichment
- Prospecting
- Webhook
- MCP
- AI Agents
- United Kingdom
---
