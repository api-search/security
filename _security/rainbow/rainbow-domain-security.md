---
api_specs:
- filename: rainbow-applications-api-openapi.yml
  format: yaml
  label: Rainbow Applications API
  slug: rainbow-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-applications-api-openapi.yml
- filename: rainbow-authentication-api-openapi.yml
  format: yaml
  label: Rainbow Authentication API
  slug: rainbow-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-authentication-api-openapi.yml
- filename: rainbow-bubbles-api-openapi.yml
  format: yaml
  label: Rainbow Bubbles API
  slug: rainbow-bubbles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-bubbles-api-openapi.yml
- filename: rainbow-contacts-api-openapi.yml
  format: yaml
  label: Rainbow Contacts API
  slug: rainbow-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-contacts-api-openapi.yml
- filename: rainbow-conversations-api-openapi.yml
  format: yaml
  label: Rainbow Conversations API
  slug: rainbow-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-conversations-api-openapi.yml
- filename: rainbow-messages-api-openapi.yml
  format: yaml
  label: Rainbow Messages API
  slug: rainbow-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-messages-api-openapi.yml
- filename: rainbow-users-api-openapi.yml
  format: yaml
  label: Rainbow Users API
  slug: rainbow-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/openapi/rainbow-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openrainbow.com
  spf: true
hosts:
- cert_expires: Sep 19 11:01:59 2026 GMT
  host: www.openrainbow.com
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: developers.openrainbow.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: openrainbow.com
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rainbow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rainbow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rainbow
provider_slug: rainbow
slug: rainbow-domain-security
source_filename: rainbow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openrainbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:01:59 2026 GMT\n  hsts: true\n  hsts_max_age: 157680000\n- host: developers.openrainbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: openrainbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: openrainbow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/security/rainbow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- CPaaS
- Chat
- Voice
- Video
- Telephony
- Messaging
- Collaboration
- Unified Communications
---
