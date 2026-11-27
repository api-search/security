---
api_specs:
- filename: paidnice-com-action-api-openapi.yml
  format: yaml
  label: Paidnice Action API
  slug: paidnice-com-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-action-api-openapi.yml
- filename: paidnice-com-contact-api-openapi.yml
  format: yaml
  label: Paidnice Contact API
  slug: paidnice-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-contact-api-openapi.yml
- filename: paidnice-com-inbound-api-openapi.yml
  format: yaml
  label: Paidnice Inbound API
  slug: paidnice-com-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-inbound-api-openapi.yml
- filename: paidnice-com-invoice-api-openapi.yml
  format: yaml
  label: Paidnice Invoice API
  slug: paidnice-com-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-invoice-api-openapi.yml
- filename: paidnice-com-note-api-openapi.yml
  format: yaml
  label: Paidnice Note API
  slug: paidnice-com-note-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-note-api-openapi.yml
- filename: paidnice-com-organisation-api-openapi.yml
  format: yaml
  label: Paidnice Organisation API
  slug: paidnice-com-organisation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-organisation-api-openapi.yml
- filename: paidnice-com-stripe-payment-api-openapi.yml
  format: yaml
  label: Paidnice Stripe Payment API
  slug: paidnice-com-stripe-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-stripe-payment-api-openapi.yml
- filename: paidnice-com-user-api-openapi.yml
  format: yaml
  label: Paidnice User API
  slug: paidnice-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidnice-com/openapi/paidnice-com-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paidnice.com
  spf: true
hosts:
- cert_expires: Feb  5 22:29:36 2027 GMT
  host: paidnice.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Paidnice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paidnice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paidnice
provider_slug: paidnice-com
slug: paidnice-com-domain-security
source_filename: paidnice-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paidnice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 22:29:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: paidnice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/paidnice-com/security/paidnice-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AR Automation
- Accounting
- Payments
- Artificial Intelligence
- Software-as-a-Service
---
