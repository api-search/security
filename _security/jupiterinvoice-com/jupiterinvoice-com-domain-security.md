---
api_specs:
- filename: jupiterinvoice-com-customers-api-openapi.yml
  format: yaml
  label: JupiterInvoice Customers API
  slug: jupiterinvoice-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiterinvoice-com/openapi/jupiterinvoice-com-customers-api-openapi.yml
- filename: jupiterinvoice-com-invoices-api-openapi.yml
  format: yaml
  label: JupiterInvoice Invoices API
  slug: jupiterinvoice-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiterinvoice-com/openapi/jupiterinvoice-com-invoices-api-openapi.yml
- filename: jupiterinvoice-com-webhooks-api-openapi.yml
  format: yaml
  label: JupiterInvoice Webhooks API
  slug: jupiterinvoice-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jupiterinvoice-com/openapi/jupiterinvoice-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jupiterinvoice.com
  spf: true
hosts:
- cert_expires: Jan  6 08:35:47 2027 GMT
  host: jupiterinvoice.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JupiterInvoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JupiterInvoice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: JupiterInvoice
provider_slug: jupiterinvoice-com
slug: jupiterinvoice-com-domain-security
source_filename: jupiterinvoice-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jupiterinvoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 08:35:47 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jupiterinvoice.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/jupiterinvoice-com/security/jupiterinvoice-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Invoicing
- Fintech
- Software-as-a-Service
- Free
---
