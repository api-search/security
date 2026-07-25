---
api_specs:
- filename: circana-brands-api-openapi.yml
  format: yaml
  label: Circana Brands API
  slug: circana-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-brands-api-openapi.yml
- filename: circana-categories-api-openapi.yml
  format: yaml
  label: Circana Categories API
  slug: circana-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-categories-api-openapi.yml
- filename: circana-consumer-panel-api-openapi.yml
  format: yaml
  label: Circana Consumer Panel API
  slug: circana-consumer-panel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-consumer-panel-api-openapi.yml
- filename: circana-exports-api-openapi.yml
  format: yaml
  label: Circana Exports API
  slug: circana-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-exports-api-openapi.yml
- filename: circana-market-data-api-openapi.yml
  format: yaml
  label: Circana Market Data API
  slug: circana-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-market-data-api-openapi.yml
- filename: circana-reports-api-openapi.yml
  format: yaml
  label: Circana Reports API
  slug: circana-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-reports-api-openapi.yml
- filename: circana-retailers-api-openapi.yml
  format: yaml
  label: Circana Retailers API
  slug: circana-retailers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/openapi/circana-retailers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:infosecalerts@circana.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: circana.com
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: www.circana.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.circana.com
  https: false
kind: domain-security
layout: security
method: probed
name: Circana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circana, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Circana
provider_slug: circana
slug: circana-domain-security
source_filename: circana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.circana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.circana.com\n  https: false\ndomains:\n- domain: circana.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:infosecalerts@circana.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/security/circana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
---
