---
api_specs:
- filename: sendar-app-emails-api-openapi.yml
  format: yaml
  label: sendar-app Emails API
  slug: sendar-app-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-emails-api-openapi.yml
- filename: sendar-app-headless-api-openapi.yml
  format: yaml
  label: sendar-app Headless API
  slug: sendar-app-headless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-headless-api-openapi.yml
- filename: sendar-app-inboxes-api-openapi.yml
  format: yaml
  label: sendar-app Inboxes API
  slug: sendar-app-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-inboxes-api-openapi.yml
- filename: sendar-app-link-checks-api-openapi.yml
  format: yaml
  label: sendar-app Link Checks API
  slug: sendar-app-link-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendar-app/openapi/sendar-app-link-checks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sendar.app
  spf: true
hosts:
- cert_expires: Dec 29 03:49:59 2026 GMT
  host: sendar.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sendar App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sendar-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: sendar-app
provider_slug: sendar-app
slug: sendar-app-domain-security
source_filename: sendar-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendar.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 03:49:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sendar.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sendar-app/security/sendar-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Delivery
- API
- Automation
---
