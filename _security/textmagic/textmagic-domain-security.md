---
api_specs:
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Messages API
  slug: textmagic-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Bulk Messaging API
  slug: textmagic-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Chats and Replies API
  slug: textmagic-chats-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Contacts and Lists API
  slug: textmagic-contacts-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Templates API
  slug: textmagic-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Scheduled Messages API
  slug: textmagic-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
- filename: textmagic-openapi.yml
  format: yaml
  label: Textmagic Sender IDs and Numbers API
  slug: textmagic-senderids-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/openapi/textmagic-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "starfieldtech.com"
  - 0 iodef "mailto:security@textmagic.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: textmagic.com
  spf: true
hosts:
- cert_expires: Dec 26 14:41:07 2026 GMT
  host: www.textmagic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 14:41:07 2026 GMT
  host: docs.textmagic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 14:41:07 2026 GMT
  host: rest.textmagic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Textmagic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Textmagic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Textmagic
provider_slug: textmagic
slug: textmagic-domain-security
source_filename: textmagic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.textmagic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 14:41:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.textmagic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 14:41:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.textmagic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 14:41:07 2026 GMT\n  hsts: null\ndomains:\n- domain: textmagic.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 iodef \"mailto:security@textmagic.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/textmagic/refs/heads/main/security/textmagic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SMS
- Text Messaging
- Messaging
- Communications
- CPaaS
---
