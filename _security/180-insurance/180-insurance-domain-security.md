---
api_specs:
- filename: 180-insurance-cota-es-api-openapi.yml
  format: yaml
  label: 180 Insurance Cotações API
  slug: 180-insurance-cota-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-cota-es-api-openapi.yml
- filename: 180-insurance-produtos-api-openapi.yml
  format: yaml
  label: 180 Insurance Produtos API
  slug: 180-insurance-produtos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-produtos-api-openapi.yml
- filename: 180-insurance-propostas-api-openapi.yml
  format: yaml
  label: 180 Insurance Propostas API
  slug: 180-insurance-propostas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-propostas-api-openapi.yml
- filename: 180-insurance-renova-es-api-openapi.yml
  format: yaml
  label: 180 Insurance Renovações API
  slug: 180-insurance-renova-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-renova-es-api-openapi.yml
- filename: 180-insurance-sinistros-api-openapi.yml
  format: yaml
  label: 180 Insurance Sinistros API
  slug: 180-insurance-sinistros-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-sinistros-api-openapi.yml
- filename: 180-insurance-vendas-api-openapi.yml
  format: yaml
  label: 180 Insurance Vendas API
  slug: 180-insurance-vendas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-vendas-api-openapi.yml
- filename: 180-insurance-webhooks-api-openapi.yml
  format: yaml
  label: 180 Insurance Webhooks API
  slug: 180-insurance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 180s.com.br
  spf: true
hosts:
- cert_expires: Sep 30 18:12:09 2026 GMT
  host: 180s.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 180 Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 180 Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 180 Insurance
provider_slug: 180-insurance
slug: 180-insurance-domain-security
source_filename: 180-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 180s.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:12:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 180s.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/security/180-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Insurance
- Embedded Insurance
- Brazil
- Fintech
- Webhook
---
