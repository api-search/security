---
api_specs:
- filename: impri-dev-actions-api-openapi.yml
  format: yaml
  label: Impri Actions API
  slug: impri-dev-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-actions-api-openapi.yml
- filename: impri-dev-billing-api-openapi.yml
  format: yaml
  label: Impri Billing API
  slug: impri-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-billing-api-openapi.yml
- filename: impri-dev-keys-api-openapi.yml
  format: yaml
  label: Impri Keys API
  slug: impri-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-keys-api-openapi.yml
- filename: impri-dev-notification-channels-api-openapi.yml
  format: yaml
  label: Impri Notification Channels API
  slug: impri-dev-notification-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-notification-channels-api-openapi.yml
- filename: impri-dev-project-api-openapi.yml
  format: yaml
  label: Impri Project API
  slug: impri-dev-project-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-project-api-openapi.yml
- filename: impri-dev-push-api-openapi.yml
  format: yaml
  label: Impri Push API
  slug: impri-dev-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-push-api-openapi.yml
- filename: impri-dev-watchers-api-openapi.yml
  format: yaml
  label: Impri Watchers API
  slug: impri-dev-watchers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-watchers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: impri.dev
  spf: true
hosts:
- cert_expires: Feb  3 16:12:36 2027 GMT
  host: impri.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Impri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Impri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Impri
provider_slug: impri-dev
slug: impri-dev-domain-security
source_filename: impri-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: impri.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 16:12:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: impri.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/impri-dev/security/impri-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Human-in-the-Loop
- Approval
- Automation
- Software-as-a-Service
---
