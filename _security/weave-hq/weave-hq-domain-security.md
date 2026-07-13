---
api_specs:
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Messaging API
  slug: weave-hq-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Phone & Calls API
  slug: weave-hq-phone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Contacts API
  slug: weave-hq-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Scheduling & Appointments API
  slug: weave-hq-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Payments API
  slug: weave-hq-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Digital Forms API
  slug: weave-hq-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Reviews API
  slug: weave-hq-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Events & Subscriptions API
  slug: weave-hq-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getweave.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: weaveconnect.com
  spf: false
hosts:
- cert_expires: Oct  6 05:54:40 2026 GMT
  host: www.getweave.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:12:01 2026 GMT
  host: dp.getweave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 00:05:58 2026 GMT
  host: api.weaveconnect.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weave Hq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weave, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weave
provider_slug: weave-hq
slug: weave-hq-domain-security
source_filename: weave-hq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:54:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dp.getweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weaveconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 00:05:58 2026 GMT\n  hsts: null\ndomains:\n- domain: getweave.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: weaveconnect.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/security/weave-hq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communication
- Healthcare
- VoIP
- Messaging
- SMS
- Scheduling
- Payments
- Reviews
- Dental
- Veterinary
---
