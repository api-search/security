---
api_specs:
- filename: pushcut-automation-server-api-openapi.yml
  format: yaml
  label: Pushcut Automation Server API
  slug: pushcut-automation-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-automation-server-api-openapi.yml
- filename: pushcut-notifications-api-openapi.yml
  format: yaml
  label: Pushcut Notifications API
  slug: pushcut-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-notifications-api-openapi.yml
- filename: pushcut-subscriptions-api-openapi.yml
  format: yaml
  label: Pushcut Subscriptions API
  slug: pushcut-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pushcut/openapi/pushcut-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pushcut.io
  spf: true
hosts:
- cert_expires: Jan  7 16:24:02 2027 GMT
  host: pushcut.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pushcut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pushcut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pushcut
provider_slug: pushcut
slug: pushcut-domain-security
source_filename: pushcut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pushcut.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 16:24:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: pushcut.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pushcut/security/pushcut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- automation
- iOS
- shortcuts
- webhooks
- integration
---
