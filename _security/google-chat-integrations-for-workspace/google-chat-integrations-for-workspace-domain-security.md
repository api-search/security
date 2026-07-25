---
api_specs:
- filename: google-chat-integrations-for-workspace-customemojis-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace CustomEmojis API
  slug: google-chat-integrations-for-workspace-customemojis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-customemojis-api-openapi.yml
- filename: google-chat-integrations-for-workspace-google-chat-api-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Google Chat API API
  slug: google-chat-integrations-for-workspace-google-chat-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-google-chat-api-api-openapi.yml
- filename: google-chat-integrations-for-workspace-members-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Members API
  slug: google-chat-integrations-for-workspace-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-members-api-openapi.yml
- filename: google-chat-integrations-for-workspace-message-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Message API
  slug: google-chat-integrations-for-workspace-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-message-api-openapi.yml
- filename: google-chat-integrations-for-workspace-messages-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Messages API
  slug: google-chat-integrations-for-workspace-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-messages-api-openapi.yml
- filename: google-chat-integrations-for-workspace-reactions-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Reactions API
  slug: google-chat-integrations-for-workspace-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-reactions-api-openapi.yml
- filename: google-chat-integrations-for-workspace-spaces-api-openapi.yml
  format: yaml
  label: Google Chat Integrations for Workspace Spaces API
  slug: google-chat-integrations-for-workspace-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/openapi/google-chat-integrations-for-workspace-spaces-api-openapi.yml
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
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: workspace.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: chat.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Chat Integrations For Workspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Chat Integrations for Workspace, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Chat Integrations for Workspace
provider_slug: google-chat-integrations-for-workspace
slug: google-chat-integrations-for-workspace-domain-security
source_filename: google-chat-integrations-for-workspace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workspace.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: chat.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-chat-integrations-for-workspace/refs/heads/main/security/google-chat-integrations-for-workspace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Google Workspace
- Team Chat
- Messaging
- Collaboration
- Chat Apps
- Spaces
- Slash Commands
- Bots
---
