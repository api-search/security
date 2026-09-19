---
api_specs:
- filename: pontofato-apis-json-api-openapi.yml
  format: yaml
  label: PontoFato Apis.json API
  slug: pontofato-apis-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-apis-json-api-openapi.yml
- filename: pontofato-buscar-api-openapi.yml
  format: yaml
  label: PontoFato Buscar API
  slug: pontofato-buscar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-buscar-api-openapi.yml
- filename: pontofato-cep-api-openapi.yml
  format: yaml
  label: PontoFato Cep API
  slug: pontofato-cep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-cep-api-openapi.yml
- filename: pontofato-contact-api-openapi.yml
  format: yaml
  label: PontoFato Contact API
  slug: pontofato-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-contact-api-openapi.yml
- filename: pontofato-credito-api-openapi.yml
  format: yaml
  label: PontoFato Credito API
  slug: pontofato-credito-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-credito-api-openapi.yml
- filename: pontofato-empresas-api-openapi.yml
  format: yaml
  label: PontoFato Empresas API
  slug: pontofato-empresas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-empresas-api-openapi.yml
- filename: pontofato-health-api-openapi.yml
  format: yaml
  label: PontoFato Health API
  slug: pontofato-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-health-api-openapi.yml
- filename: pontofato-local-api-openapi.yml
  format: yaml
  label: PontoFato Local API
  slug: pontofato-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-local-api-openapi.yml
- filename: pontofato-mcp-api-openapi.yml
  format: yaml
  label: PontoFato MCP API
  slug: pontofato-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-mcp-api-openapi.yml
- filename: pontofato-metrics-api-openapi.yml
  format: yaml
  label: PontoFato Metrics API
  slug: pontofato-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-metrics-api-openapi.yml
- filename: pontofato-okf-api-openapi.yml
  format: yaml
  label: PontoFato Okf API
  slug: pontofato-okf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-okf-api-openapi.yml
- filename: pontofato-pontofato-api-openapi.yml
  format: yaml
  label: PontoFato Ponto Fato API
  slug: pontofato-pontofato-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-pontofato-api-openapi.yml
- filename: pontofato-proximo-api-openapi.yml
  format: yaml
  label: PontoFato Proximo API
  slug: pontofato-proximo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-proximo-api-openapi.yml
- filename: pontofato-raio-api-openapi.yml
  format: yaml
  label: PontoFato Raio API
  slug: pontofato-raio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-raio-api-openapi.yml
- filename: pontofato-vizinhanca-api-openapi.yml
  format: yaml
  label: PontoFato Vizinhanca API
  slug: pontofato-vizinhanca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-vizinhanca-api-openapi.yml
- filename: pontofato-well-known-api-openapi.yml
  format: yaml
  label: PontoFato .well Known API
  slug: pontofato-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/openapi/pontofato-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pontofato.com
  spf: true
hosts:
- cert_expires: Nov 29 14:41:36 2026 GMT
  host: pontofato.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pontofato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PontoFato, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PontoFato
provider_slug: pontofato
slug: pontofato-domain-security
source_filename: pontofato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pontofato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 14:41:36 2026 GMT\n  hsts: false\ndomains:\n- domain: pontofato.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pontofato/refs/heads/main/security/pontofato-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Brazilian CEP
- address geocoding
- IBGE CNEFE
- Geospatial
- latitude/longitude
- CNPJ
- Receita Federal
- Business Registry
- Location Intelligence
- proximity search
- radius search
- Open Government Data
- agent-native
- MCP
- x402-micropayments
---
