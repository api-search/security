---
api_specs:
- filename: print-one-address-api-openapi.yml
  format: yaml
  label: print-one Address API
  slug: print-one-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-address-api-openapi.yml
- filename: print-one-campaigns-api-openapi.yml
  format: yaml
  label: print-one Campaigns API
  slug: print-one-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-campaigns-api-openapi.yml
- filename: print-one-coupons-api-openapi.yml
  format: yaml
  label: print-one Coupons API
  slug: print-one-coupons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-coupons-api-openapi.yml
- filename: print-one-design-previews-api-openapi.yml
  format: yaml
  label: print-one Design Previews API
  slug: print-one-design-previews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-design-previews-api-openapi.yml
- filename: print-one-designs-api-openapi.yml
  format: yaml
  label: print-one Designs API
  slug: print-one-designs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-designs-api-openapi.yml
- filename: print-one-imports-api-openapi.yml
  format: yaml
  label: print-one Imports API
  slug: print-one-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-imports-api-openapi.yml
- filename: print-one-items-api-openapi.yml
  format: yaml
  label: print-one Items API
  slug: print-one-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-items-api-openapi.yml
- filename: print-one-mailings-api-openapi.yml
  format: yaml
  label: print-one Mailings API
  slug: print-one-mailings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-mailings-api-openapi.yml
- filename: print-one-webhooks-api-openapi.yml
  format: yaml
  label: print-one Webhooks API
  slug: print-one-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-webhooks-api-openapi.yml
- filename: print-one-webhook-events-api-openapi.yml
  format: yaml
  label: print-one Webhook Events API
  slug: print-one-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/print-one/openapi/print-one-webhook-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: print.one
  spf: true
hosts:
- cert_expires: Dec 17 15:46:41 2026 GMT
  host: print.one
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Print One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for print-one, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: print-one
provider_slug: print-one
slug: print-one-domain-security
source_filename: print-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: print.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 15:46:41 2026 GMT\n  hsts: false\ndomains:\n- domain: print.one\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/print-one/security/print-one-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Postcards
- API
- Direct Mail
- Marketing
- Automation
---
