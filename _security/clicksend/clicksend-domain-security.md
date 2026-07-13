---
api_specs:
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend SMS API
  slug: clicksend-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend MMS API
  slug: clicksend-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Voice / Text-to-Speech API
  slug: clicksend-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Transactional Email API
  slug: clicksend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Post - Letters API
  slug: clicksend-post-letters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Post - Postcards API
  slug: clicksend-post-postcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Contacts & Lists API
  slug: clicksend-contacts-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Delivery Receipts & Inbound API
  slug: clicksend-delivery-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Account & Balance API
  slug: clicksend-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clicksend.com
  spf: true
hosts:
- cert_expires: Aug 24 20:43:31 2026 GMT
  host: www.clicksend.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: developers.clicksend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 03:28:03 2026 GMT
  host: rest.clicksend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clicksend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClickSend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClickSend
provider_slug: clicksend
slug: clicksend-domain-security
source_filename: clicksend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clicksend.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 20:43:31 2026 GMT\n  hsts: false\n- host: developers.clicksend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: rest.clicksend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:28:03 2026 GMT\n  hsts: false\ndomains:\n- domain: clicksend.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/security/clicksend-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Communications
- SMS
- MMS
- Voice
- Email
- Post
- Messaging
- CPaaS
---
