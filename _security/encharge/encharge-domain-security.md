---
api_specs:
- filename: encharge-openapi.yml
  format: yaml
  label: Encharge REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/_original/encharge-openapi.yml
- filename: TVRj5o3E
  format: yaml
  label: Encharge Transactional Email API
  slug: transactional-email-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/460427/TVRj5o3E
- filename: SVfNwVFU
  format: yaml
  label: Encharge Ingest API
  slug: ingest-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/460427/SVfNwVFU
- filename: encharge-account-api-openapi.yml
  format: yaml
  label: Encharge Account API
  slug: encharge-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-account-api-openapi.yml
- filename: encharge-broadcasts-api-openapi.yml
  format: yaml
  label: Encharge Broadcasts API
  slug: encharge-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-broadcasts-api-openapi.yml
- filename: encharge-customobjects-api-openapi.yml
  format: yaml
  label: Encharge Custom Objects API
  slug: encharge-customobjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-customobjects-api-openapi.yml
- filename: encharge-customobjectsschema-api-openapi.yml
  format: yaml
  label: Encharge Custom Objects Schema API
  slug: encharge-customobjectsschema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-customobjectsschema-api-openapi.yml
- filename: encharge-emailtemplates-api-openapi.yml
  format: yaml
  label: Encharge Email Templates API
  slug: encharge-emailtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-emailtemplates-api-openapi.yml
- filename: encharge-folders-api-openapi.yml
  format: yaml
  label: Encharge Folders API
  slug: encharge-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-folders-api-openapi.yml
- filename: encharge-people-api-openapi.yml
  format: yaml
  label: Encharge People API
  slug: encharge-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-people-api-openapi.yml
- filename: encharge-personfields-api-openapi.yml
  format: yaml
  label: Encharge Person Fields API
  slug: encharge-personfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-personfields-api-openapi.yml
- filename: encharge-segments-api-openapi.yml
  format: yaml
  label: Encharge Segments API
  slug: encharge-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-segments-api-openapi.yml
- filename: encharge-settings-api-openapi.yml
  format: yaml
  label: Encharge Email Domain Settings API
  slug: encharge-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-settings-api-openapi.yml
- filename: encharge-tags-api-openapi.yml
  format: yaml
  label: Encharge Tags API
  slug: encharge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-api-openapi.yml
- filename: encharge-tags-management-api-openapi.yml
  format: yaml
  label: Encharge Tags Management API
  slug: encharge-tags-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-tags-management-api-openapi.yml
- filename: encharge-webhooks-api-openapi.yml
  format: yaml
  label: Encharge Webhooks API
  slug: encharge-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/openapi/encharge-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: encharge.io
  spf: true
hosts:
- cert_expires: Oct  2 11:47:00 2026 GMT
  host: encharge.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 12:54:27 2026 GMT
  host: docs.encharge.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 13:29:02 2026 GMT
  host: api.encharge.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Encharge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Encharge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Encharge
provider_slug: encharge
slug: encharge-domain-security
source_filename: encharge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: encharge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:47:00 2026 GMT\n  hsts: false\n- host: docs.encharge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 12:54:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.encharge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:29:02 2026 GMT\n  hsts: false\ndomains:\n- domain: encharge.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encharge/refs/heads/main/security/encharge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Marketing Automation
- Transactional Email
- Software-as-a-Service
- Behavioral Email
- Customer Engagement
- Customer Data
- Webhook
---
