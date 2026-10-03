---
api_specs:
- filename: conta-azul-categorias-api-openapi.yml
  format: yaml
  label: Conta Azul Categorias API
  slug: conta-azul-categorias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-categorias-api-openapi.yml
- filename: conta-azul-centro-de-custo-api-openapi.yml
  format: yaml
  label: Conta Azul Centro De Custo API
  slug: conta-azul-centro-de-custo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-centro-de-custo-api-openapi.yml
- filename: conta-azul-conta-financeira-api-openapi.yml
  format: yaml
  label: Conta Azul Conta Financeira API
  slug: conta-azul-conta-financeira-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-conta-financeira-api-openapi.yml
- filename: conta-azul-contratos-api-openapi.yml
  format: yaml
  label: Conta Azul Contratos API
  slug: conta-azul-contratos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-contratos-api-openapi.yml
- filename: conta-azul-financeiro-api-openapi.yml
  format: yaml
  label: Conta Azul Financeiro API
  slug: conta-azul-financeiro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-financeiro-api-openapi.yml
- filename: conta-azul-orcamentos-api-openapi.yml
  format: yaml
  label: Conta Azul Orcamentos API
  slug: conta-azul-orcamentos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-orcamentos-api-openapi.yml
- filename: conta-azul-produto-api-openapi.yml
  format: yaml
  label: Conta Azul Produto API
  slug: conta-azul-produto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-produto-api-openapi.yml
- filename: conta-azul-protocolo-api-openapi.yml
  format: yaml
  label: Conta Azul Protocolo API
  slug: conta-azul-protocolo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-protocolo-api-openapi.yml
- filename: conta-azul-venda-api-openapi.yml
  format: yaml
  label: Conta Azul Venda API
  slug: conta-azul-venda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-venda-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: contaazul.com
  spf: true
hosts:
- cert_expires: Mar 25 12:44:22 2027 GMT
  host: contaazul.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: developers.contaazul.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 09:32:06 2026 GMT
  host: api-v2.contaazul.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Conta Azul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conta Azul, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Conta Azul
provider_slug: conta-azul
slug: conta-azul-domain-security
source_filename: conta-azul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contaazul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 25 12:44:22 2027 GMT\n  hsts: false\n- host: developers.contaazul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: false\n- host: api-v2.contaazul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:32:06 2026 GMT\n  hsts: null\ndomains:\n- domain: contaazul.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/security/conta-azul-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Accounting
- ERP
- Brazil
- Small Business
- Financial Management
- Invoicing
- Payments
---
