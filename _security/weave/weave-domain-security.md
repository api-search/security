---
api_specs:
- filename: weave-contacts-api-openapi.yml
  format: yaml
  label: Weave Contacts API
  slug: weave-hq-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/openapi/weave-contacts-api-openapi.yml
- filename: weave-events-api-openapi.yml
  format: yaml
  label: Weave Events API
  slug: weave-hq-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/openapi/weave-events-api-openapi.yml
- filename: weave-forms-api-openapi.yml
  format: yaml
  label: Weave Forms API
  slug: weave-hq-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/openapi/weave-forms-api-openapi.yml
- filename: weave-messaging-api-openapi.yml
  format: yaml
  label: Weave Messaging API
  slug: weave-hq-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/openapi/weave-messaging-api-openapi.yml
- filename: weave-payments-api-openapi.yml
  format: yaml
  label: Weave Payments API
  slug: weave-hq-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/openapi/weave-payments-api-openapi.yml
- filename: weave-phone-calls-api-openapi.yml
  format: yaml
  label: Weave Phone & Calls API
  slug: weave-hq-phone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/openapi/weave-phone-calls-api-openapi.yml
- filename: weave-reviews-api-openapi.yml
  format: yaml
  label: Weave Reviews API
  slug: weave-hq-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/openapi/weave-reviews-api-openapi.yml
- filename: weave-scheduling-api-openapi.yml
  format: yaml
  label: Weave Scheduling API
  slug: weave-hq-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/openapi/weave-scheduling-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
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
- cert_expires: Oct 13 17:27:14 2026 GMT
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
name: Weave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weave, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weave
provider_slug: weave
slug: weave-domain-security
source_filename: weave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 17:27:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dp.getweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.weaveconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 00:05:58 2026 GMT\n  hsts: null\ndomains:\n- domain: getweave.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: weaveconnect.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weave/refs/heads/main/security/weave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Communications
- Messaging
- Payments
- Healthcare
- VoIP
- Telephony
- Reviews
- Scheduling
- SMB
- Developer Platform
- Authentication
---
