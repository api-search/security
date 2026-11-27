---
api_specs:
- filename: google-chat-spaces-api-openapi.yml
  format: yaml
  label: Google Chat Spaces API
  slug: google-chat-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat/openapi/google-chat-spaces-api-openapi.yml
- filename: google-chat-media-api-openapi.yml
  format: yaml
  label: Google Chat Chat Media API
  slug: google-chat-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat/openapi/google-chat-media-api-openapi.yml
- filename: google-chat-users-api-openapi.yml
  format: yaml
  label: Google Chat Chat Users API
  slug: google-chat-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat/openapi/google-chat-users-api-openapi.yml
- filename: google-chat-custom-emojis-api-openapi.yml
  format: yaml
  label: Google Chat Custom Emojis API
  slug: google-chat-custom-emojis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-chat/openapi/google-chat-custom-emojis-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: chat.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Chat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Chat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Chat
provider_slug: google-chat
slug: google-chat-domain-security
source_filename: google-chat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: chat.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-chat/security/google-chat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat
- Collaboration
- Google
- Google Workspace
- Messaging
- Spaces
---
