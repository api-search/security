---
api_specs:
- filename: cayra-io-admin-api-openapi.yml
  format: yaml
  label: Cayra Admin API
  slug: cayra-io-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-admin-api-openapi.yml
- filename: cayra-io-admin-vm-pool-api-openapi.yml
  format: yaml
  label: Cayra Admin Vm Pool API
  slug: cayra-io-admin-vm-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-admin-vm-pool-api-openapi.yml
- filename: cayra-io-agreements-api-openapi.yml
  format: yaml
  label: Cayra Agreements API
  slug: cayra-io-agreements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-agreements-api-openapi.yml
- filename: cayra-io-billing-api-openapi.yml
  format: yaml
  label: Cayra Billing API
  slug: cayra-io-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-billing-api-openapi.yml
- filename: cayra-io-cayra-license-server-api-openapi.yml
  format: yaml
  label: Cayra Cayra License Server API
  slug: cayra-io-cayra-license-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-cayra-license-server-api-openapi.yml
- filename: cayra-io-client-api-openapi.yml
  format: yaml
  label: Cayra Client API
  slug: cayra-io-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-client-api-openapi.yml
- filename: cayra-io-deployments-api-openapi.yml
  format: yaml
  label: Cayra Deployments API
  slug: cayra-io-deployments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-deployments-api-openapi.yml
- filename: cayra-io-health-api-openapi.yml
  format: yaml
  label: Cayra Health API
  slug: cayra-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-health-api-openapi.yml
- filename: cayra-io-messaging-api-openapi.yml
  format: yaml
  label: Cayra Messaging API
  slug: cayra-io-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-messaging-api-openapi.yml
- filename: cayra-io-mobile-invite-api-openapi.yml
  format: yaml
  label: Cayra Mobile Invite API
  slug: cayra-io-mobile-invite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-mobile-invite-api-openapi.yml
- filename: cayra-io-plaud-webhook-api-openapi.yml
  format: yaml
  label: Cayra Plaud Webhook API
  slug: cayra-io-plaud-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-plaud-webhook-api-openapi.yml
- filename: cayra-io-report-feedback-api-openapi.yml
  format: yaml
  label: Cayra Report Feedback API
  slug: cayra-io-report-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-report-feedback-api-openapi.yml
- filename: cayra-io-self-service-api-openapi.yml
  format: yaml
  label: Cayra Self Service API
  slug: cayra-io-self-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-self-service-api-openapi.yml
- filename: cayra-io-stripe-api-openapi.yml
  format: yaml
  label: Cayra Stripe API
  slug: cayra-io-stripe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-stripe-api-openapi.yml
- filename: cayra-io-stripe-webhook-api-openapi.yml
  format: yaml
  label: Cayra Stripe Webhook API
  slug: cayra-io-stripe-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-stripe-webhook-api-openapi.yml
- filename: cayra-io-usage-api-openapi.yml
  format: yaml
  label: Cayra Usage API
  slug: cayra-io-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-usage-api-openapi.yml
- filename: cayra-io-whatsapp-routing-api-openapi.yml
  format: yaml
  label: Cayra Whatsapp Routing API
  slug: cayra-io-whatsapp-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-whatsapp-routing-api-openapi.yml
- filename: cayra-io-whatsapp-webhook-api-openapi.yml
  format: yaml
  label: Cayra Whatsapp Webhook API
  slug: cayra-io-whatsapp-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cayra-io/openapi/cayra-io-whatsapp-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cayra.io
  spf: true
hosts:
- cert_expires: Jan 30 00:16:18 2027 GMT
  host: cayra.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cayra Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cayra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cayra
provider_slug: cayra-io
slug: cayra-io-domain-security
source_filename: cayra-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cayra.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 00:16:18 2027 GMT\n  hsts: false\ndomains:\n- domain: cayra.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cayra-io/security/cayra-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Enterprise
- Decision Intelligence
- ERP
- Database
---
