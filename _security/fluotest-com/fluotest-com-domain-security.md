---
api_specs:
- filename: fluotest-com-mcp-api-openapi.yml
  format: yaml
  label: FluoTest MCP API
  slug: fluotest-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluotest-com/openapi/fluotest-com-mcp-api-openapi.yml
- filename: fluotest-com-status-api-openapi.yml
  format: yaml
  label: FluoTest Status API
  slug: fluotest-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluotest-com/openapi/fluotest-com-status-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fluotest.com
  spf: true
hosts:
- cert_expires: Jan 24 20:49:36 2027 GMT
  host: fluotest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FluoTest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FluoTest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FluoTest
provider_slug: fluotest-com
slug: fluotest-com-domain-security
source_filename: fluotest-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluotest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 20:49:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fluotest.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fluotest-com/security/fluotest-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Quiz
- No-Code
- Education
- Marketing
---
