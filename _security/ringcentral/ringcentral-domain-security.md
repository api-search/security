---
api_specs:
- filename: ringcentral-platform-openapi.yml
  format: yaml
  label: RingCentral Voice API
  slug: ringcentral-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/openapi/ringcentral-platform-openapi.yml
- filename: ringcentral-subscriptions-asyncapi.yaml
  format: yaml
  label: RingCentral Webhooks and Subscriptions API
  slug: ringcentral-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/asyncapi/ringcentral-subscriptions-asyncapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ringcentral.com
  spf: true
hosts:
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: www.ringcentral.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: platform.ringcentral.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: media.ringcentral.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ringcentral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RingCentral, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RingCentral
provider_slug: ringcentral
slug: ringcentral-domain-security
source_filename: ringcentral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ringcentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.ringcentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\n- host: media.ringcentral.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ringcentral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/security/ringcentral-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- UCaaS
- Voice
- Video
- Contact Center
- SMS
- Messaging
- Fax
---
