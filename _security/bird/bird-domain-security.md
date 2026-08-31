---
api_specs:
- filename: bird-faq-api-openapi.yml
  format: yaml
  label: Bird FAQ API
  slug: bird-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-faq-api-openapi.yml
- filename: bird-intent-api-openapi.yml
  format: yaml
  label: Bird Intent API
  slug: bird-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-intent-api-openapi.yml
- filename: bird-languagedetection-api-openapi.yml
  format: yaml
  label: Bird LanguageDetection API
  slug: bird-languagedetection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-languagedetection-api-openapi.yml
- filename: bird-namedentityrecognition-api-openapi.yml
  format: yaml
  label: Bird NamedEntityRecognition API
  slug: bird-namedentityrecognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-namedentityrecognition-api-openapi.yml
- filename: bird-sms-messaging-api-openapi.yml
  format: yaml
  label: Bird SMS Messaging API
  slug: bird-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-sms-messaging-api-openapi.yml
- filename: bird-channels-api-openapi.yml
  format: yaml
  label: Bird Channels API
  slug: bird-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-channels-api-openapi.yml
- filename: bird-contacts-api-openapi.yml
  format: yaml
  label: Bird Contacts API
  slug: bird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-contacts-api-openapi.yml
- filename: bird-conversations-api-openapi.yml
  format: yaml
  label: Bird Conversations API
  slug: bird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-conversations-api-openapi.yml
- filename: bird-legacy-messagebird-api-openapi.yml
  format: yaml
  label: Bird Legacy MessageBird API
  slug: bird-legacy-messagebird-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-legacy-messagebird-api-openapi.yml
- filename: bird-messaging-api-openapi.yml
  format: yaml
  label: Bird Messaging API
  slug: bird-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-messaging-api-openapi.yml
- filename: bird-numbers-api-openapi.yml
  format: yaml
  label: Bird Numbers API
  slug: bird-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/openapi/bird-numbers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  - 0 issue "usertrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bird.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: bird.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:26:11 2026 GMT
  host: docs.bird.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api.bird.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bird, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bird
provider_slug: bird
slug: bird-domain-security
source_filename: bird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.bird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:26:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bird.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issue \"usertrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bird/refs/heads/main/security/bird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- SMS
- Email
- WhatsApp
- Voice
- Messaging
- Omnichannel
- Customer Engagement
---
