---
api_specs:
- filename: splitit-authentication-api-openapi.yml
  format: yaml
  label: Splitit Authentication API
  slug: splitit-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitit/refs/heads/main/openapi/splitit-authentication-api-openapi.yml
- filename: splitit-eligibility-api-openapi.yml
  format: yaml
  label: Splitit Eligibility API
  slug: splitit-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitit/refs/heads/main/openapi/splitit-eligibility-api-openapi.yml
- filename: splitit-installment-plans-api-openapi.yml
  format: yaml
  label: Splitit Installment Plans API
  slug: splitit-installment-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitit/refs/heads/main/openapi/splitit-installment-plans-api-openapi.yml
- filename: splitit-merchant-management-api-openapi.yml
  format: yaml
  label: Splitit Merchant Management API
  slug: splitit-merchant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splitit/refs/heads/main/openapi/splitit-merchant-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: splitit.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: developers.splitit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: webapi.production.splitit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: web-api-v3.sandbox.splitit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Splitit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splitit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Splitit
provider_slug: splitit
slug: splitit-domain-security
source_filename: splitit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.splitit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\n- host: webapi.production.splitit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\n- host: web-api-v3.sandbox.splitit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: splitit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splitit/refs/heads/main/security/splitit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Installments
- Buy Now Pay Later
- Credit Card
- Fintech
- E-Commerce
---
