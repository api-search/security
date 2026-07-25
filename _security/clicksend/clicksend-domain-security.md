---
api_specs:
- filename: clicksend-account-api-openapi.yml
  format: yaml
  label: ClickSend Account API
  slug: clicksend-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-account-api-openapi.yml
- filename: clicksend-contact-api-openapi.yml
  format: yaml
  label: ClickSend Contact API
  slug: clicksend-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-contact-api-openapi.yml
- filename: clicksend-contactlist-api-openapi.yml
  format: yaml
  label: ClickSend ContactList API
  slug: clicksend-contactlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-contactlist-api-openapi.yml
- filename: clicksend-email-api-openapi.yml
  format: yaml
  label: ClickSend Email API
  slug: clicksend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-email-api-openapi.yml
- filename: clicksend-mms-api-openapi.yml
  format: yaml
  label: ClickSend MMS API
  slug: clicksend-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-mms-api-openapi.yml
- filename: clicksend-post-letter-api-openapi.yml
  format: yaml
  label: ClickSend Post Letter API
  slug: clicksend-post-letter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-post-letter-api-openapi.yml
- filename: clicksend-post-postcard-api-openapi.yml
  format: yaml
  label: ClickSend Post Postcard API
  slug: clicksend-post-postcard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-post-postcard-api-openapi.yml
- filename: clicksend-receipts-api-openapi.yml
  format: yaml
  label: ClickSend Receipts API
  slug: clicksend-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-receipts-api-openapi.yml
- filename: clicksend-sms-api-openapi.yml
  format: yaml
  label: ClickSend SMS API
  slug: clicksend-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-sms-api-openapi.yml
- filename: clicksend-voice-api-openapi.yml
  format: yaml
  label: ClickSend Voice API
  slug: clicksend-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-voice-api-openapi.yml
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
