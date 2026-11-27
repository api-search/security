---
api_specs:
- filename: codeatlas-com-br-contact-api-openapi.yml
  format: yaml
  label: CodeAtlas Contact API
  slug: codeatlas-com-br-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-contact-api-openapi.yml
- filename: codeatlas-com-br-discovery-api-openapi.yml
  format: yaml
  label: CodeAtlas Discovery API
  slug: codeatlas-com-br-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-discovery-api-openapi.yml
- filename: codeatlas-com-br-exports-api-openapi.yml
  format: yaml
  label: CodeAtlas Exports API
  slug: codeatlas-com-br-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-exports-api-openapi.yml
- filename: codeatlas-com-br-oauth-api-openapi.yml
  format: yaml
  label: CodeAtlas OAuth API
  slug: codeatlas-com-br-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-oauth-api-openapi.yml
- filename: codeatlas-com-br-system-api-openapi.yml
  format: yaml
  label: CodeAtlas System API
  slug: codeatlas-com-br-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-system-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: codeatlas.com.br
  spf: true
hosts:
- cert_expires: Feb  1 05:21:44 2027 GMT
  host: codeatlas.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CodeAtlas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeAtlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CodeAtlas
provider_slug: codeatlas-com-br
slug: codeatlas-com-br-domain-security
source_filename: codeatlas-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codeatlas.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 05:21:44 2027 GMT\n  hsts: false\ndomains:\n- domain: codeatlas.com.br\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/codeatlas-com-br/security/codeatlas-com-br-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Software Development
- Developer Tools
- AI Agents
- MCP
- Custom Software
- Brazil
---
