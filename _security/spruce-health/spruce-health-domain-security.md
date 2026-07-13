---
api_specs:
- filename: spruce-health-openapi.yml
  format: yaml
  label: Spruce Contacts API
  slug: spruce-health-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-openapi.yml
- filename: spruce-health-openapi.yml
  format: yaml
  label: Spruce Conversations API
  slug: spruce-health-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-openapi.yml
- filename: spruce-health-openapi.yml
  format: yaml
  label: Spruce Messages API
  slug: spruce-health-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-openapi.yml
- filename: spruce-health-openapi.yml
  format: yaml
  label: Spruce Webhooks API
  slug: spruce-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@sprucehealth.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
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
  hsts: null
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
overview: 'Domain security posture for Spruce Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spruce Health
provider_slug: spruce-health
slug: spruce-health-domain-security
source_filename: spruce-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sprucehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sprucehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:30:33 2026 GMT\n  hsts: null\n- host: api.sprucehealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sprucehealth.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@sprucehealth.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/security/spruce-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- HIPAA
- Communication
- Secure Messaging
- Telehealth
- Contacts
- Conversations
- Messaging
- Webhooks
- VoIP
---
