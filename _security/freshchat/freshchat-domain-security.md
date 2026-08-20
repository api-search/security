---
api_specs:
- filename: freshchat-accounts-api-openapi.yml
  format: yaml
  label: Freshchat Accounts API
  slug: freshchat-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-accounts-api-openapi.yml
- filename: freshchat-agents-api-openapi.yml
  format: yaml
  label: Freshchat Agents API
  slug: freshchat-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-agents-api-openapi.yml
- filename: freshchat-businesshours-api-openapi.yml
  format: yaml
  label: Freshchat BusinessHours API
  slug: freshchat-businesshours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-businesshours-api-openapi.yml
- filename: freshchat-channels-api-openapi.yml
  format: yaml
  label: Freshchat Channels API
  slug: freshchat-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-channels-api-openapi.yml
- filename: freshchat-conversations-api-openapi.yml
  format: yaml
  label: Freshchat Conversations API
  slug: freshchat-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-conversations-api-openapi.yml
- filename: freshchat-csat-api-openapi.yml
  format: yaml
  label: Freshchat CSAT API
  slug: freshchat-csat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-csat-api-openapi.yml
- filename: freshchat-files-api-openapi.yml
  format: yaml
  label: Freshchat Files API
  slug: freshchat-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-files-api-openapi.yml
- filename: freshchat-groups-api-openapi.yml
  format: yaml
  label: Freshchat Groups API
  slug: freshchat-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-groups-api-openapi.yml
- filename: freshchat-messages-api-openapi.yml
  format: yaml
  label: Freshchat Messages API
  slug: freshchat-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-messages-api-openapi.yml
- filename: freshchat-metrics-api-openapi.yml
  format: yaml
  label: Freshchat Metrics API
  slug: freshchat-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-metrics-api-openapi.yml
- filename: freshchat-outboundmessages-api-openapi.yml
  format: yaml
  label: Freshchat OutboundMessages API
  slug: freshchat-outboundmessages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-outboundmessages-api-openapi.yml
- filename: freshchat-roles-api-openapi.yml
  format: yaml
  label: Freshchat Roles API
  slug: freshchat-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-roles-api-openapi.yml
- filename: freshchat-users-api-openapi.yml
  format: yaml
  label: Freshchat Users API
  slug: freshchat-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freshworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freshchat.com
  spf: true
hosts:
- cert_expires: Aug 22 10:30:03 2026 GMT
  host: www.freshworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: developers.freshchat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 13:31:52 2026 GMT
  host: api.freshchat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshchat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freshchat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freshchat
provider_slug: freshchat
slug: freshchat-domain-security
source_filename: freshchat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freshworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:30:03 2026 GMT\n  hsts: null\n- host: developers.freshchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.freshchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 13:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freshworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: freshchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/security/freshchat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Messaging
- Live Chat
- Customer-Support
- Conversational Engagement
- Omnichannel Messaging
- Chatbots
- Freshworks
---
