---
api_specs:
- filename: convertkit-accounts-api-openapi.yml
  format: yaml
  label: Kit Accounts API
  slug: convertkit-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-accounts-api-openapi.yml
- filename: convertkit-broadcasts-api-openapi.yml
  format: yaml
  label: Kit Broadcasts API
  slug: convertkit-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-broadcasts-api-openapi.yml
- filename: convertkit-custom-fields-api-openapi.yml
  format: yaml
  label: Kit Custom Fields API
  slug: convertkit-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-custom-fields-api-openapi.yml
- filename: convertkit-email-templates-api-openapi.yml
  format: yaml
  label: Kit Email Templates API
  slug: convertkit-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-email-templates-api-openapi.yml
- filename: convertkit-forms-api-openapi.yml
  format: yaml
  label: Kit Forms API
  slug: convertkit-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-forms-api-openapi.yml
- filename: convertkit-posts-api-openapi.yml
  format: yaml
  label: Kit Posts API
  slug: convertkit-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-posts-api-openapi.yml
- filename: convertkit-purchases-api-openapi.yml
  format: yaml
  label: Kit Purchases API
  slug: convertkit-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-purchases-api-openapi.yml
- filename: convertkit-segments-api-openapi.yml
  format: yaml
  label: Kit Segments API
  slug: convertkit-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-segments-api-openapi.yml
- filename: convertkit-sequence-emails-api-openapi.yml
  format: yaml
  label: Kit Sequence Emails API
  slug: convertkit-sequence-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequence-emails-api-openapi.yml
- filename: convertkit-sequences-api-openapi.yml
  format: yaml
  label: Kit Sequences API
  slug: convertkit-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequences-api-openapi.yml
- filename: convertkit-snippets-api-openapi.yml
  format: yaml
  label: Kit Snippets API
  slug: convertkit-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-snippets-api-openapi.yml
- filename: convertkit-subscribers-api-openapi.yml
  format: yaml
  label: Kit Subscribers API
  slug: convertkit-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-subscribers-api-openapi.yml
- filename: convertkit-tags-api-openapi.yml
  format: yaml
  label: Kit Tags API
  slug: convertkit-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-tags-api-openapi.yml
- filename: convertkit-webhooks-api-openapi.yml
  format: yaml
  label: Kit Webhooks API
  slug: convertkit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kit.com
  spf: true
hosts:
- cert_expires: Nov  4 10:00:01 2026 GMT
  host: kit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 17:14:03 2026 GMT
  host: developers.kit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: api.kit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Convertkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kit
provider_slug: convertkit
slug: convertkit-domain-security
source_filename: convertkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 10:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.kit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 17:14:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.kit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/security/convertkit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Creator Economy
- Subscribers
- Automation
- Newsletters
- Sequences
- Forms
- Broadcasts
- Webhook
- MCP
- Agents
- Authentication
- Marketing Automation
- Landing Pages
- Segmentation
- Email Campaigns
- Software-as-a-Service
- Commerce
---
