---
api_specs:
- filename: brevo-transactional-email-openapi.yml
  format: yaml
  label: Brevo Transactional Email API
  slug: transactional-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-transactional-email-openapi.yml
- filename: brevo-email-campaigns-openapi.yml
  format: yaml
  label: Brevo Email Campaigns API
  slug: email-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-email-campaigns-openapi.yml
- filename: brevo-contacts-openapi.yml
  format: yaml
  label: Brevo Contacts API
  slug: contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-contacts-openapi.yml
- filename: brevo-transactional-sms-openapi.yml
  format: yaml
  label: Brevo Transactional SMS API
  slug: transactional-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-transactional-sms-openapi.yml
- filename: brevo-whatsapp-openapi.yml
  format: yaml
  label: Brevo WhatsApp API
  slug: whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-whatsapp-openapi.yml
- filename: brevo-ecommerce-openapi.yml
  format: yaml
  label: Brevo eCommerce API
  slug: ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-ecommerce-openapi.yml
- filename: brevo-conversations-openapi.yml
  format: yaml
  label: Brevo Conversations API
  slug: conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-conversations-openapi.yml
- filename: brevo-webhooks-openapi.yml
  format: yaml
  label: Brevo Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/openapi/brevo-webhooks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brevo.com
  spf: true
hosts:
- cert_expires: Sep 20 18:16:10 2026 GMT
  host: developers.brevo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 16:29:24 2026 GMT
  host: api.brevo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brevo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for brevo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: brevo
provider_slug: brevo
slug: brevo-domain-security
source_filename: brevo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.brevo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:16:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.brevo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:29:24 2026 GMT\n  hsts: null\ndomains:\n- domain: brevo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brevo/refs/heads/main/security/brevo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
