---
api_specs:
- filename: thanks-io-creatives-library-api-openapi.yml
  format: yaml
  label: Thanks.io Creatives Library API
  slug: thanks-io-creatives-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-creatives-library-api-openapi.yml
- filename: thanks-io-dynamic-images-api-openapi.yml
  format: yaml
  label: Thanks.io Dynamic Images API
  slug: thanks-io-dynamic-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-dynamic-images-api-openapi.yml
- filename: thanks-io-giftcards-api-openapi.yml
  format: yaml
  label: Thanks.io Giftcards API
  slug: thanks-io-giftcards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-giftcards-api-openapi.yml
- filename: thanks-io-handwriting-styles-api-openapi.yml
  format: yaml
  label: Thanks.io Handwriting Styles API
  slug: thanks-io-handwriting-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-handwriting-styles-api-openapi.yml
- filename: thanks-io-image-templates-api-openapi.yml
  format: yaml
  label: Thanks.io Image Templates API
  slug: thanks-io-image-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-image-templates-api-openapi.yml
- filename: thanks-io-mailing-lists-api-openapi.yml
  format: yaml
  label: Thanks.io Mailing Lists API
  slug: thanks-io-mailing-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-mailing-lists-api-openapi.yml
- filename: thanks-io-message-templates-api-openapi.yml
  format: yaml
  label: Thanks.io Message Templates API
  slug: thanks-io-message-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-message-templates-api-openapi.yml
- filename: thanks-io-order-estimates-api-openapi.yml
  format: yaml
  label: Thanks.io Order Estimates API
  slug: thanks-io-order-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-order-estimates-api-openapi.yml
- filename: thanks-io-orders-api-openapi.yml
  format: yaml
  label: Thanks.io Orders API
  slug: thanks-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-orders-api-openapi.yml
- filename: thanks-io-recipients-api-openapi.yml
  format: yaml
  label: Thanks.io Recipients API
  slug: thanks-io-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-recipients-api-openapi.yml
- filename: thanks-io-send-mailer-api-openapi.yml
  format: yaml
  label: Thanks.io Send Mailer API
  slug: thanks-io-send-mailer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-send-mailer-api-openapi.yml
- filename: thanks-io-webhook-events-api-openapi.yml
  format: yaml
  label: Thanks.io Webhook Events API
  slug: thanks-io-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-webhook-events-api-openapi.yml
- filename: thanks-io-webhooks-api-openapi.yml
  format: yaml
  label: Thanks.io Webhooks API
  slug: thanks-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-webhooks-api-openapi.yml
- filename: thanks-io-subaccounts-api-openapi.yml
  format: yaml
  label: Thanks.io Subaccounts API
  slug: thanks-io-subaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-subaccounts-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thanks.io
  spf: true
hosts:
- cert_expires: Jan  6 23:22:23 2027 GMT
  host: thanks.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thanks Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thanks.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Thanks.io
provider_slug: thanks-io
slug: thanks-io-domain-security
source_filename: thanks-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thanks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:22:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thanks.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/thanks-io/security/thanks-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- DirectMail
- Automation
- API
---
