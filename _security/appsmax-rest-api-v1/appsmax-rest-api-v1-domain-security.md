---
api_specs:
- filename: appsmax-rest-api-v1-access-api-openapi.yml
  format: yaml
  label: AppsMax Access API
  slug: appsmax-rest-api-v1-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-access-api-openapi.yml
- filename: appsmax-rest-api-v1-applications-api-openapi.yml
  format: yaml
  label: AppsMax Applications API
  slug: appsmax-rest-api-v1-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-applications-api-openapi.yml
- filename: appsmax-rest-api-v1-bots-api-openapi.yml
  format: yaml
  label: AppsMax Bots API
  slug: appsmax-rest-api-v1-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-bots-api-openapi.yml
- filename: appsmax-rest-api-v1-campaigns-api-openapi.yml
  format: yaml
  label: AppsMax Campaigns API
  slug: appsmax-rest-api-v1-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-campaigns-api-openapi.yml
- filename: appsmax-rest-api-v1-funnels-api-openapi.yml
  format: yaml
  label: AppsMax Funnels API
  slug: appsmax-rest-api-v1-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-funnels-api-openapi.yml
- filename: appsmax-rest-api-v1-interactive-menu-api-openapi.yml
  format: yaml
  label: AppsMax Interactive menu API
  slug: appsmax-rest-api-v1-interactive-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-interactive-menu-api-openapi.yml
- filename: appsmax-rest-api-v1-miniapps-api-openapi.yml
  format: yaml
  label: AppsMax Miniapps API
  slug: appsmax-rest-api-v1-miniapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-miniapps-api-openapi.yml
- filename: appsmax-rest-api-v1-organizations-api-openapi.yml
  format: yaml
  label: AppsMax Organizations API
  slug: appsmax-rest-api-v1-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-organizations-api-openapi.yml
- filename: appsmax-rest-api-v1-subscribers-api-openapi.yml
  format: yaml
  label: AppsMax Subscribers API
  slug: appsmax-rest-api-v1-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-subscribers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appsmax.ru
  spf: true
hosts:
- cert_expires: Nov  5 13:33:45 2026 GMT
  host: appsmax.ru
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 03:32:22 2026 GMT
  host: telegram.appsmax.ru
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appsmax Rest Api V1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppsMax, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AppsMax
provider_slug: appsmax-rest-api-v1
slug: appsmax-rest-api-v1-domain-security
source_filename: appsmax-rest-api-v1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appsmax.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 13:33:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: telegram.appsmax.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:32:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appsmax.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/security/appsmax-rest-api-v1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software-as-a-Service
- Messaging
- Business Automation
- Chatbots
- Mini Apps
- Customer Requests
- Workflow-Automation
- MAX
- Telegram
- Russian Language
---
