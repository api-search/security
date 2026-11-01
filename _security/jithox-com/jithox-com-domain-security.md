---
api_specs:
- filename: jithox-com-iban-api-openapi.yml
  format: yaml
  label: jithox-com Iban API
  slug: jithox-com-iban-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-iban-api-openapi.yml
- filename: jithox-com-invoice-api-openapi.yml
  format: yaml
  label: jithox-com Invoice API
  slug: jithox-com-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-invoice-api-openapi.yml
- filename: jithox-com-payment-api-openapi.yml
  format: yaml
  label: jithox-com Payment API
  slug: jithox-com-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-payment-api-openapi.yml
- filename: jithox-com-peppol-api-openapi.yml
  format: yaml
  label: jithox-com Peppol API
  slug: jithox-com-peppol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-peppol-api-openapi.yml
- filename: jithox-com-vat-api-openapi.yml
  format: yaml
  label: jithox-com Vat API
  slug: jithox-com-vat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jithox-com/openapi/jithox-com-vat-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jithox.com
  spf: true
hosts:
- cert_expires: Nov 28 08:56:56 2026 GMT
  host: jithox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jithox Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jithox-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: jithox-com
provider_slug: jithox-com
slug: jithox-com-domain-security
source_filename: jithox-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jithox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 08:56:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jithox.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jithox-com/security/jithox-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Automation
- BackOffice
- Tools
---
