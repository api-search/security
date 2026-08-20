---
api_specs:
- filename: mailerlite-automations-api-openapi.yml
  format: yaml
  label: MailerLite Automations API
  slug: mailerlite-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-automations-api-openapi.yml
- filename: mailerlite-campaigns-api-openapi.yml
  format: yaml
  label: MailerLite Campaigns API
  slug: mailerlite-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-campaigns-api-openapi.yml
- filename: mailerlite-fields-api-openapi.yml
  format: yaml
  label: MailerLite Fields API
  slug: mailerlite-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-fields-api-openapi.yml
- filename: mailerlite-forms-api-openapi.yml
  format: yaml
  label: MailerLite Forms API
  slug: mailerlite-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-forms-api-openapi.yml
- filename: mailerlite-groups-api-openapi.yml
  format: yaml
  label: MailerLite Groups API
  slug: mailerlite-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-groups-api-openapi.yml
- filename: mailerlite-segments-api-openapi.yml
  format: yaml
  label: MailerLite Segments API
  slug: mailerlite-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-segments-api-openapi.yml
- filename: mailerlite-subscribers-api-openapi.yml
  format: yaml
  label: MailerLite Subscribers API
  slug: mailerlite-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-subscribers-api-openapi.yml
- filename: mailerlite-webhooks-api-openapi.yml
  format: yaml
  label: MailerLite Webhooks API
  slug: mailerlite-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailerlite.com
  spf: true
hosts:
- cert_expires: Sep 15 09:56:40 2026 GMT
  host: www.mailerlite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 11:46:24 2026 GMT
  host: developers.mailerlite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: classic.developers.mailerlite.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mailerlite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailerLite, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MailerLite
provider_slug: mailerlite
slug: mailerlite-domain-security
source_filename: mailerlite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailerlite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:56:40 2026 GMT\n  hsts: null\n- host: developers.mailerlite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 11:46:24 2026 GMT\n  hsts: false\n- host: classic.developers.mailerlite.com\n  https: false\ndomains:\n- domain: mailerlite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/security/mailerlite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email Marketing
- Automation
- Newsletters
- Subscribers
- Campaigns
- Webhook
- E-Commerce
- Segmentation
- Transactional Email
- MCP
---
