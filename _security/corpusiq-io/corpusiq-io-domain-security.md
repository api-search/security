---
api_specs:
- filename: corpusiq-io-authentication-api-openapi.yml
  format: yaml
  label: CorpusIQ Authentication API
  slug: corpusiq-io-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiq-io/openapi/corpusiq-io-authentication-api-openapi.yml
- filename: corpusiq-io-discovery-api-openapi.yml
  format: yaml
  label: CorpusIQ Discovery API
  slug: corpusiq-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiq-io/openapi/corpusiq-io-discovery-api-openapi.yml
- filename: corpusiq-io-mcp-api-openapi.yml
  format: yaml
  label: CorpusIQ MCP API
  slug: corpusiq-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiq-io/openapi/corpusiq-io-mcp-api-openapi.yml
- filename: corpusiq-io-usage-api-openapi.yml
  format: yaml
  label: CorpusIQ Usage API
  slug: corpusiq-io-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corpusiq-io/openapi/corpusiq-io-usage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corpusiq.io
  spf: true
hosts:
- cert_expires: Jan 26 02:05:49 2027 GMT
  host: corpusiq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CorpusIQ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CorpusIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CorpusIQ
provider_slug: corpusiq-io
slug: corpusiq-io-domain-security
source_filename: corpusiq-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corpusiq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 02:05:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corpusiq.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/corpusiq-io/security/corpusiq-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- MCP
- Business Intelligence
- Small Business
- Integration
- ChatGPT
- Analytics
---
