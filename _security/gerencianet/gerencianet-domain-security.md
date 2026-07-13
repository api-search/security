---
api_specs:
- filename: efi-cobrancas-openapi.yml
  format: yaml
  label: Efí Pay Cobranças API
  slug: efi-cobrancas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-cobrancas-openapi.yml
- filename: efi-pix-openapi.yml
  format: yaml
  label: Efí Pay Pix API
  slug: efi-pix
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-pix-openapi.yml
- filename: efi-openfinance-openapi.yml
  format: yaml
  label: Efí Pay Open Finance API
  slug: efi-openfinance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-openfinance-openapi.yml
- filename: efi-contas-openapi.yml
  format: yaml
  label: Efí Pay Contas (Account Opening) API
  slug: efi-contas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-contas-openapi.yml
- filename: efi-pagamentos-openapi.yml
  format: yaml
  label: Efí Pay Pagamentos (Bill Payment) API
  slug: efi-pagamentos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-pagamentos-openapi.yml
- filename: efi-extratos-openapi.yml
  format: yaml
  label: Efí Pay Extratos (Statements) API
  slug: efi-extratos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/openapi/efi-extratos-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sejaefi.com.br
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: efipay.com.br
  spf: true
hosts:
- cert_expires: Aug 14 11:15:13 2026 GMT
  host: sejaefi.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 17:16:54 2026 GMT
  host: cobrancas.api.efipay.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 17:16:54 2026 GMT
  host: cobrancas-h.api.efipay.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gerencianet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Efí Pay (Gerencianet), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Efí Pay (Gerencianet)
provider_slug: gerencianet
slug: gerencianet-domain-security
source_filename: gerencianet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sejaefi.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 11:15:13 2026 GMT\n  hsts: false\n- host: cobrancas.api.efipay.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 17:16:54 2026 GMT\n  hsts: null\n- host: cobrancas-h.api.efipay.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 17:16:54 2026 GMT\n  hsts: null\ndomains:\n- domain: sejaefi.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: efipay.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gerencianet/refs/heads/main/security/gerencianet-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Payments
- Pix
- Boleto
- Subscriptions
- Recurring Billing
- Marketplace
- Split Payments
- Open Finance
- Banking as a Service
- Account Opening
- Bill Payment
- CNAB
- Brazil
- Fintech
---
