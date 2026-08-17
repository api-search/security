---
api_specs:
- filename: simpletexting-campaigns-api-openapi.yml
  format: yaml
  label: SimpleTexting Campaigns API
  slug: simpletexting-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-campaigns-api-openapi.yml
- filename: simpletexting-contact-lists-api-openapi.yml
  format: yaml
  label: SimpleTexting Contact Lists API
  slug: simpletexting-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contact-lists-api-openapi.yml
- filename: simpletexting-contact-segments-api-openapi.yml
  format: yaml
  label: SimpleTexting Contact Segments API
  slug: simpletexting-contact-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contact-segments-api-openapi.yml
- filename: simpletexting-contacts-api-openapi.yml
  format: yaml
  label: SimpleTexting Contacts API
  slug: simpletexting-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contacts-api-openapi.yml
- filename: simpletexting-contacts-batch-operations-api-openapi.yml
  format: yaml
  label: SimpleTexting Contacts - Batch Operations API
  slug: simpletexting-contacts-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contacts-batch-operations-api-openapi.yml
- filename: simpletexting-custom-fields-api-openapi.yml
  format: yaml
  label: SimpleTexting Custom Fields API
  slug: simpletexting-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-custom-fields-api-openapi.yml
- filename: simpletexting-media-items-api-openapi.yml
  format: yaml
  label: SimpleTexting Media Items API
  slug: simpletexting-media-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-media-items-api-openapi.yml
- filename: simpletexting-messages-api-openapi.yml
  format: yaml
  label: SimpleTexting Messages API
  slug: simpletexting-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-messages-api-openapi.yml
- filename: simpletexting-tenant-api-openapi.yml
  format: yaml
  label: SimpleTexting Tenant API
  slug: simpletexting-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-tenant-api-openapi.yml
- filename: simpletexting-webhooks-api-openapi.yml
  format: yaml
  label: SimpleTexting Webhooks API
  slug: simpletexting-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-webhooks-api-openapi.yml
- filename: simpletexting-tenant-phones-api-openapi.yml
  format: yaml
  label: SimpleTexting Tenant phones API
  slug: simpletexting-tenant-phones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-tenant-phones-api-openapi.yml
- filename: simpletexting-webhook-reports-api-openapi.yml
  format: yaml
  label: SimpleTexting Webhook Reports API
  slug: simpletexting-webhook-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-webhook-reports-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: simpletexting.com
  spf: true
hosts:
- cert_expires: Oct 18 04:04:25 2026 GMT
  host: simpletexting.com
  hsts: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api-doc.simpletexting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api-app2.simpletexting.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simpletexting Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleTexting, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SimpleTexting
provider_slug: simpletexting
slug: simpletexting-domain-security
source_filename: simpletexting-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simpletexting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 04:04:25 2026 GMT\n  hsts: true\n- host: api-doc.simpletexting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-app2.simpletexting.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: simpletexting.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/security/simpletexting-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SMS
- MMS
- Messaging
- Marketing
- Text Messaging
- SMS Marketing
- Communications
- Campaigns
- Contacts
- Webhooks
- A2P 10DLC
---
