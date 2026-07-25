---
api_specs:
- filename: sentio-ai-api-openapi.yml
  format: yaml
  label: Sentio AI API
  slug: sentio-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-ai-api-openapi.yml
- filename: sentio-alerts-api-openapi.yml
  format: yaml
  label: Sentio Alerts API
  slug: sentio-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-alerts-api-openapi.yml
- filename: sentio-data-api-openapi.yml
  format: yaml
  label: Sentio Data API
  slug: sentio-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-data-api-openapi.yml
- filename: sentio-debug-and-simulation-api-openapi.yml
  format: yaml
  label: Sentio Debug and Simulation API
  slug: sentio-debug-and-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-debug-and-simulation-api-openapi.yml
- filename: sentio-forks-api-openapi.yml
  format: yaml
  label: Sentio Forks API
  slug: sentio-forks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-forks-api-openapi.yml
- filename: sentio-move-api-openapi.yml
  format: yaml
  label: Sentio Move API
  slug: sentio-move-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-move-api-openapi.yml
- filename: sentio-price-api-openapi.yml
  format: yaml
  label: Sentio Price API
  slug: sentio-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-price-api-openapi.yml
- filename: sentio-prices-api-openapi.yml
  format: yaml
  label: Sentio Prices API
  slug: sentio-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-prices-api-openapi.yml
- filename: sentio-processor-api-openapi.yml
  format: yaml
  label: Sentio Processor API
  slug: sentio-processor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-processor-api-openapi.yml
- filename: sentio-processorext-api-openapi.yml
  format: yaml
  label: Sentio ProcessorExt API
  slug: sentio-processorext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-processorext-api-openapi.yml
- filename: sentio-web-api-openapi.yml
  format: yaml
  label: Sentio Web API
  slug: sentio-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/openapi/sentio-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sentio.xyz
  spf: true
hosts:
- cert_expires: Oct 18 10:15:47 2026 GMT
  host: api.sentio.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sentio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sentio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sentio
provider_slug: sentio
slug: sentio-domain-security
source_filename: sentio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.sentio.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 10:15:47 2026 GMT\n  hsts: null\ndomains:\n- domain: sentio.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentio/refs/heads/main/security/sentio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web3
- Blockchain
- Observability
- Analytics
- Data
- Indexing
- Monitoring
- Developer Tools
- Crypto
- API
---
