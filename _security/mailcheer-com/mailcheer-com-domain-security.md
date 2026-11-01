---
api_specs:
- filename: mailcheer-com-campaigns-api-openapi.yml
  format: yaml
  label: mailcheer-com Campaigns API
  slug: mailcheer-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcheer-com/openapi/mailcheer-com-campaigns-api-openapi.yml
- filename: mailcheer-com-emails-api-openapi.yml
  format: yaml
  label: mailcheer-com Emails API
  slug: mailcheer-com-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcheer-com/openapi/mailcheer-com-emails-api-openapi.yml
- filename: mailcheer-com-subscribers-api-openapi.yml
  format: yaml
  label: mailcheer-com Subscribers API
  slug: mailcheer-com-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcheer-com/openapi/mailcheer-com-subscribers-api-openapi.yml
- filename: mailcheer-com-suppression-api-openapi.yml
  format: yaml
  label: mailcheer-com Suppression API
  slug: mailcheer-com-suppression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcheer-com/openapi/mailcheer-com-suppression-api-openapi.yml
- filename: mailcheer-com-webhooks-api-openapi.yml
  format: yaml
  label: mailcheer-com Webhooks API
  slug: mailcheer-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcheer-com/openapi/mailcheer-com-webhooks-api-openapi.yml
- filename: mailcheer-com-workspace-api-openapi.yml
  format: yaml
  label: mailcheer-com Workspace API
  slug: mailcheer-com-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailcheer-com/openapi/mailcheer-com-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mailcheer.com
  spf: true
hosts:
- cert_expires: Dec 21 08:32:19 2026 GMT
  host: mailcheer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailcheer Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailcheer-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mailcheer-com
provider_slug: mailcheer-com
slug: mailcheer-com-domain-security
source_filename: mailcheer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailcheer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 08:32:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailcheer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mailcheer-com/security/mailcheer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Newsletter
- API
- Marketing
- AI
---
