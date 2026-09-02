---
api_specs:
- filename: faturapdf-brazilian-invoice-receipt-pdf-api-documents-api-openapi.yml
  format: yaml
  label: FaturaPDF — Brazilian Invoice & Receipt PDF API Documents API
  slug: faturapdf-brazilian-invoice-receipt-pdf-api-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faturapdf-brazilian-invoice-receipt-pdf-api/refs/heads/main/openapi/faturapdf-brazilian-invoice-receipt-pdf-api-documents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: faturapdf.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Oct 25 02:29:59 2026 GMT
  host: faturapdf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: brazilian-invoice-receipt-pdf-api-cpf-cnpj.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Faturapdf Brazilian Invoice Receipt Pdf Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FaturaPDF — Brazilian Invoice & Receipt PDF API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: FaturaPDF — Brazilian Invoice & Receipt PDF API
provider_slug: faturapdf-brazilian-invoice-receipt-pdf-api
slug: faturapdf-brazilian-invoice-receipt-pdf-api-domain-security
source_filename: faturapdf-brazilian-invoice-receipt-pdf-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faturapdf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 02:29:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: brazilian-invoice-receipt-pdf-api-cpf-cnpj.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: faturapdf.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faturapdf-brazilian-invoice-receipt-pdf-api/refs/heads/main/security/faturapdf-brazilian-invoice-receipt-pdf-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Invoices
- Receipts
- PDF Generation
- Documents
- Brazil
- Billing
- CPF Validation
- CNPJ Validation
- Pix
- Fintech
- Data Validation
---
