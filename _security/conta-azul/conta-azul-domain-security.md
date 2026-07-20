---
api_specs:
- filename: conta-azul-acquittance-openapi.yml
  format: yaml
  label: Conta Azul Baixas (Acquittance)
  slug: conta-azul-baixas-acquittance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-acquittance-openapi.yml
- filename: conta-azul-charge-openapi.yml
  format: yaml
  label: Conta Azul Cobranças (Charges)
  slug: conta-azul-cobranças-charges
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-charge-openapi.yml
- filename: conta-azul-contracts-openapi.yml
  format: yaml
  label: Conta Azul Contratos (Contracts)
  slug: conta-azul-contratos-contracts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-contracts-openapi.yml
- filename: conta-azul-financial-openapi.yml
  format: yaml
  label: Conta Azul Financeiro (Financial)
  slug: conta-azul-financeiro-financial
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-financial-openapi.yml
- filename: conta-azul-inventory-openapi.yml
  format: yaml
  label: Conta Azul Produtos (Inventory)
  slug: conta-azul-produtos-inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-inventory-openapi.yml
- filename: conta-azul-proposal-openapi.yml
  format: yaml
  label: Conta Azul Orçamentos (Proposals)
  slug: conta-azul-orçamentos-proposals
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-proposal-openapi.yml
- filename: conta-azul-protocol-openapi.yml
  format: yaml
  label: Conta Azul Protocolos (Protocol)
  slug: conta-azul-protocolos-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-protocol-openapi.yml
- filename: conta-azul-sales-openapi.yml
  format: yaml
  label: Conta Azul Vendas (Sales)
  slug: conta-azul-vendas-sales
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-sales-openapi.yml
- filename: conta-azul-scheduled-sales-openapi.yml
  format: yaml
  label: Conta Azul Vendas Programadas (Scheduled Sales)
  slug: conta-azul-vendas-programadas-scheduled-sales
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conta-azul/refs/heads/main/openapi/conta-azul-scheduled-sales-openapi.yml
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
