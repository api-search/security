---
api_specs:
- filename: wazo-auth-api-openapi.yml
  format: yaml
  label: Wazo Authentication API (wazo-auth)
  slug: wazo-authentication-api-wazo-auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-auth-api-openapi.yml
- filename: wazo-confd-api-openapi.yml
  format: yaml
  label: Wazo Configuration API (wazo-confd)
  slug: wazo-configuration-api-wazo-confd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-confd-api-openapi.yml
- filename: wazo-calld-api-openapi.yml
  format: yaml
  label: Wazo Call Control / Application API (wazo-calld)
  slug: wazo-call-control-application-api-wazo-calld
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-calld-api-openapi.yml
- filename: wazo-call-logd-api-openapi.yml
  format: yaml
  label: Wazo Call Detail Records API (wazo-call-logd)
  slug: wazo-call-detail-records-api-wazo-call-logd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-call-logd-api-openapi.yml
- filename: wazo-dird-api-openapi.yml
  format: yaml
  label: Wazo Directory & Contacts API (wazo-dird)
  slug: wazo-directory-contacts-api-wazo-dird
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-dird-api-openapi.yml
- filename: wazo-provd-api-openapi.yml
  format: yaml
  label: Wazo Phone Provisioning API (wazo-provd)
  slug: wazo-phone-provisioning-api-wazo-provd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-provd-api-openapi.yml
- filename: wazo-webhookd-api-openapi.yml
  format: yaml
  label: Wazo Webhooks API (wazo-webhookd)
  slug: wazo-webhooks-api-wazo-webhookd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-webhookd-api-openapi.yml
- filename: wazo-plugind-api-openapi.yml
  format: yaml
  label: Wazo Plugin Management API (wazo-plugind)
  slug: wazo-plugin-management-api-wazo-plugind
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-plugind-api-openapi.yml
- filename: wazo-agentd-api-openapi.yml
  format: yaml
  label: Wazo Call Centre Agent API (wazo-agentd)
  slug: wazo-call-centre-agent-api-wazo-agentd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-agentd-api-openapi.yml
- filename: wazo-chatd-api-openapi.yml
  format: yaml
  label: Wazo Presence & Chat API (wazo-chatd)
  slug: wazo-presence-chat-api-wazo-chatd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-chatd-api-openapi.yml
- filename: wazo-phoned-api-openapi.yml
  format: yaml
  label: Wazo Phone Directory & Service API (wazo-phoned)
  slug: wazo-phone-directory-service-api-wazo-phoned
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-phoned-api-openapi.yml
- filename: wazo-setupd-api-openapi.yml
  format: yaml
  label: Wazo Initial Setup API (wazo-setupd)
  slug: wazo-initial-setup-api-wazo-setupd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-setupd-api-openapi.yml
- filename: wazo-amid-api-openapi.yml
  format: yaml
  label: Wazo Asterisk Manager Interface API (wazo-amid)
  slug: wazo-asterisk-manager-interface-api-wazo-amid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/openapi/wazo-amid-api-openapi.yml
- filename: wazo-unattributed-asyncapi.yml
  format: yaml
  label: Wazo Websocket Event Stream (wazo-websocketd)
  slug: wazo-websocket-event-stream-wazo-websocketd
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/asyncapi/wazo-unattributed-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wazo.io
  spf: true
hosts:
- cert_expires: Nov  1 13:33:52 2026 GMT
  host: wazo.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:06:50 2026 GMT
  host: developers.wazo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 02:15:14 2026 GMT
  host: api.wazo.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wazo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wazo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wazo
provider_slug: wazo
slug: wazo-domain-security
source_filename: wazo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wazo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 13:33:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.wazo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:06:50 2026 GMT\n  hsts: false\n- host: api.wazo.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 02:15:14 2026 GMT\n  hsts: false\ndomains:\n- domain: wazo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wazo/refs/heads/main/security/wazo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- telephony
- voip
- unified-communications
- ucaas
- contact-center
- sip
- asterisk
- webrtc
- open-source
- self-hosted
- white-label
- pbx
- msp
- call-center
- provisioning
- webhooks
- event-driven
- chat
- presence
- cdr
---
