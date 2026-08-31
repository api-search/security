---
api_specs:
- filename: spruce-health-contact-fields-api-openapi.yml
  format: yaml
  label: Spruce Health Contact Fields API
  slug: spruce-health-contact-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contact-fields-api-openapi.yml
- filename: spruce-health-contact-tags-api-openapi.yml
  format: yaml
  label: Spruce Health Contact Tags API
  slug: spruce-health-contact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contact-tags-api-openapi.yml
- filename: spruce-health-contacts-api-openapi.yml
  format: yaml
  label: Spruce Health Contacts API
  slug: spruce-health-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contacts-api-openapi.yml
- filename: spruce-health-conversation-item-api-openapi.yml
  format: yaml
  label: Spruce Health Conversation Item API
  slug: spruce-health-conversation-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversation-item-api-openapi.yml
- filename: spruce-health-conversation-tags-api-openapi.yml
  format: yaml
  label: Spruce Health Conversation Tags API
  slug: spruce-health-conversation-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversation-tags-api-openapi.yml
- filename: spruce-health-conversations-api-openapi.yml
  format: yaml
  label: Spruce Health Conversations API
  slug: spruce-health-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversations-api-openapi.yml
- filename: spruce-health-internal-endpoints-api-openapi.yml
  format: yaml
  label: Spruce Health Internal Endpoints API
  slug: spruce-health-internal-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-internal-endpoints-api-openapi.yml
- filename: spruce-health-media-api-openapi.yml
  format: yaml
  label: Spruce Health Media API
  slug: spruce-health-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-media-api-openapi.yml
- filename: spruce-health-organization-api-openapi.yml
  format: yaml
  label: Spruce Health Organization API
  slug: spruce-health-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-organization-api-openapi.yml
- filename: spruce-health-phone-lines-api-openapi.yml
  format: yaml
  label: Spruce Health Phone Lines API
  slug: spruce-health-phone-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-phone-lines-api-openapi.yml
- filename: spruce-health-saved-messages-api-openapi.yml
  format: yaml
  label: Spruce Health Saved Messages API
  slug: spruce-health-saved-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-saved-messages-api-openapi.yml
- filename: spruce-health-scheduled-messages-api-openapi.yml
  format: yaml
  label: Spruce Health Scheduled Messages API
  slug: spruce-health-scheduled-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-scheduled-messages-api-openapi.yml
- filename: spruce-health-teams-api-openapi.yml
  format: yaml
  label: Spruce Health Teams API
  slug: spruce-health-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-teams-api-openapi.yml
- filename: spruce-health-transcription-api-openapi.yml
  format: yaml
  label: Spruce Health Transcription API
  slug: spruce-health-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-transcription-api-openapi.yml
- filename: spruce-health-webhooks-api-openapi.yml
  format: yaml
  label: Spruce Health Webhooks API
  slug: spruce-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@sprucehealth.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sprucehealth.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: sprucehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 03:30:33 2026 GMT
  host: developer.sprucehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.sprucehealth.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spruce Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spruce Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spruce Health
provider_slug: spruce-health
slug: spruce-health-domain-security
source_filename: spruce-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sprucehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sprucehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:30:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sprucehealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sprucehealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@sprucehealth.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/security/spruce-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- HIPAA
- Communications
- Secure Messaging
- Telehealth
- Patient Engagement
- Contacts
- Conversations
- Messaging
- SMS
- Voice
- VoIP
- Fax
- Video
- Webhook
- Scheduling
- Transcription
- EHR Integration
- Compliance
---
