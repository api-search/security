---
api_specs:
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Pix Charges API
  slug: efi-bank-pix-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Pix Payments API
  slug: efi-bank-pix-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Pix Webhooks API
  slug: efi-bank-pix-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Cobranças (Charges) API
  slug: efi-bank-cobrancas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Carnê API
  slug: efi-bank-carne-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
- filename: efi-bank-openapi.yml
  format: yaml
  label: Efí Pix via Open Finance API
  slug: efi-bank-open-finance-pix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/openapi/efi-bank-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sejaefi.com.br
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.salesforce.com -all
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: efipay.com.br
  spf: true
  spf_record: v=spf1 -all
hosts:
- cert_expires: Aug 14 11:15:13 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: sejaefi.com.br
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 12:21:14 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: dev.efipay.com.br
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 17:16:54 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: pix.api.efipay.com.br
  hsts: false
  https: true
  mtls_required: true
  note: Mutual TLS client certificate required; plain HTTPS request without a client cert does not return a normal HTTP response.
  tls_version: TLSv1.3
- cert_expires: Dec  6 17:16:54 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: cobrancas.api.efipay.com.br
  hsts: false
  http_status: 404
  https: true
  mtls_required: false
  note: Root path returns 404; the API is served under versioned paths (e.g. /v1/authorize).
  tls_version: TLSv1.3
- cert_expires: Dec  6 17:16:54 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: openfinance.api.efipay.com.br
  hsts: false
  https: true
  mtls_required: true
  note: Mutual TLS client certificate required on every request.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Efi Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Efí, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Efí
provider_slug: efi-bank
slug: efi-bank-domain-security
source_filename: efi-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sejaefi.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Aug 14 11:15:13 2026 GMT\n  hsts: false\n  http_status: 200\n- host: dev.efipay.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Aug 17 12:21:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  http_status: 200\n- host: pix.api.efipay.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Dec  6 17:16:54 2026 GMT\n  hsts: false\n  mtls_required: true\n  note: Mutual TLS client certificate required; plain HTTPS request without a client cert does not return a normal HTTP response.\n- host: cobrancas.api.efipay.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires:\
  \ Dec  6 17:16:54 2026 GMT\n  hsts: false\n  mtls_required: false\n  http_status: 404\n  note: Root path returns 404; the API is served under versioned paths (e.g. /v1/authorize).\n- host: openfinance.api.efipay.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Dec  6 17:16:54 2026 GMT\n  hsts: false\n  mtls_required: true\n  note: Mutual TLS client certificate required on every request.\ndomains:\n- domain: sejaefi.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.salesforce.com -all\n  dmarc: true\n  dmarc_policy: reject\n- domain: efipay.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 -all\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/efi-bank/refs/heads/main/security/efi-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Pix
- Boleto
- Banking
- Brazil
- Latin America
- Charges
- Digital Account
- Financial Infrastructure
- Fintech
---
