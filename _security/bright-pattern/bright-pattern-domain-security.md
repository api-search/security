---
api_specs:
- filename: bright-pattern-authentication-api-openapi.yml
  format: yaml
  label: Bright Pattern Authentication API
  slug: bright-pattern-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-authentication-api-openapi.yml
- filename: bright-pattern-calling-list-api-openapi.yml
  format: yaml
  label: Bright Pattern Calling List API
  slug: bright-pattern-calling-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-calling-list-api-openapi.yml
- filename: bright-pattern-campaigns-api-openapi.yml
  format: yaml
  label: Bright Pattern Campaigns API
  slug: bright-pattern-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-campaigns-api-openapi.yml
- filename: bright-pattern-dnc-lists-api-openapi.yml
  format: yaml
  label: Bright Pattern DNC Lists API
  slug: bright-pattern-dnc-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-dnc-lists-api-openapi.yml
- filename: bright-pattern-do-not-call-list-api-openapi.yml
  format: yaml
  label: Bright Pattern Do Not Call List API
  slug: bright-pattern-do-not-call-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-do-not-call-list-api-openapi.yml
- filename: bright-pattern-link-groups-api-openapi.yml
  format: yaml
  label: Bright Pattern Link Groups API
  slug: bright-pattern-link-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-link-groups-api-openapi.yml
- filename: bright-pattern-lists-api-openapi.yml
  format: yaml
  label: Bright Pattern Lists API
  slug: bright-pattern-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-lists-api-openapi.yml
- filename: bright-pattern-methods-api-openapi.yml
  format: yaml
  label: Bright Pattern Methods API
  slug: bright-pattern-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-methods-api-openapi.yml
- filename: bright-pattern-multichannel-call-recordings-api-openapi.yml
  format: yaml
  label: Bright Pattern Multichannel Call Recordings API
  slug: bright-pattern-multichannel-call-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-multichannel-call-recordings-api-openapi.yml
- filename: bright-pattern-phones-api-openapi.yml
  format: yaml
  label: Bright Pattern Phones API
  slug: bright-pattern-phones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-phones-api-openapi.yml
- filename: bright-pattern-regular-call-recordings-api-openapi.yml
  format: yaml
  label: Bright Pattern Regular Call Recordings API
  slug: bright-pattern-regular-call-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-regular-call-recordings-api-openapi.yml
- filename: bright-pattern-sms-mms-messaging-api-openapi.yml
  format: yaml
  label: Bright Pattern SMS/MMS Messaging API
  slug: bright-pattern-sms-mms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-sms-mms-messaging-api-openapi.yml
- filename: bright-pattern-task-routing-api-openapi.yml
  format: yaml
  label: Bright Pattern Task Routing API
  slug: bright-pattern-task-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-task-routing-api-openapi.yml
- filename: bright-pattern-users-api-openapi.yml
  format: yaml
  label: Bright Pattern Users API
  slug: bright-pattern-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/openapi/bright-pattern-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brightpattern.com
  spf: true
hosts:
- cert_expires: Oct  2 20:30:57 2026 GMT
  host: www.brightpattern.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: help.brightpattern.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bright Pattern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright Pattern, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bright Pattern
provider_slug: bright-pattern
slug: bright-pattern-domain-security
source_filename: bright-pattern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightpattern.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:30:57 2026 GMT\n  hsts: false\n- host: help.brightpattern.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: brightpattern.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-pattern/refs/heads/main/security/bright-pattern-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Contact Center
- CCaaS
- Customer Experience
- Omnichannel
- Call Center
- Telephony
- Messaging
- SMS
- Voice
- Customer Service
- Workforce Management
---
