---
api_specs:
- filename: augment-api-key-api-openapi.yml
  format: yaml
  label: Augment API Key API
  slug: augment-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-api-key-api-openapi.yml
- filename: augment-carrier-management-api-openapi.yml
  format: yaml
  label: Augment Carrier Management API
  slug: augment-carrier-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-carrier-management-api-openapi.yml
- filename: augment-carrier-support-api-openapi.yml
  format: yaml
  label: Augment Carrier Support API
  slug: augment-carrier-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-carrier-support-api-openapi.yml
- filename: augment-load-management-api-openapi.yml
  format: yaml
  label: Augment Load Management API
  slug: augment-load-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-load-management-api-openapi.yml
- filename: augment-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Augment Webhook Endpoints API
  slug: augment-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-webhook-endpoints-api-openapi.yml
- filename: augment-webhook-event-subscriptions-api-openapi.yml
  format: yaml
  label: Augment Webhook Event Subscriptions API
  slug: augment-webhook-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/openapi/augment-webhook-event-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goaugment.com
  spf: true
hosts:
- cert_expires: Sep 20 14:19:40 2026 GMT
  host: goaugment.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: api.prod.goaugment.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Augment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augment, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Augment
provider_slug: augment
slug: augment-domain-security
source_filename: augment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goaugment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 14:19:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.prod.goaugment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: goaugment.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augment/refs/heads/main/security/augment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Freight
- Supply Chain
- Transportation
- Webhook
- Artificial Intelligence
- Automation
---
