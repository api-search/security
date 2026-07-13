---
api_specs:
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI SMS API
  slug: smsapi-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI MMS API
  slug: smsapi-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI VMS Voice API
  slug: smsapi-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Contacts API
  slug: smsapi-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Sender Names API
  slug: smsapi-sender-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI 2FA Authentication API
  slug: smsapi-2fa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Subusers API
  slug: smsapi-subusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Profile and Account API
  slug: smsapi-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI HLR Lookup API
  slug: smsapi-hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Blacklist API
  slug: smsapi-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
- filename: smsapi-openapi.yml
  format: yaml
  label: SMSAPI Short URLs API
  slug: smsapi-short-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/openapi/smsapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smsapi.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: smsapi.eu
  spf: false
hosts:
- cert_expires: Feb  4 10:32:32 2027 GMT
  host: www.smsapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 10:32:32 2027 GMT
  host: api.smsapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: api.smsapi.eu
  https: false
kind: domain-security
layout: security
method: probed
name: Smsapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMSAPI, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SMSAPI
provider_slug: smsapi
slug: smsapi-domain-security
source_filename: smsapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 10:32:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.smsapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  4 10:32:32 2027 GMT\n  hsts: null\n- host: api.smsapi.eu\n  https: false\ndomains:\n- domain: smsapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: smsapi.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smsapi/refs/heads/main/security/smsapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- SMS
- MMS
- Voice
- 2FA
- Bulk Messaging
- Communications
- CPaaS
---
