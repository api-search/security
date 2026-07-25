---
api_specs:
- filename: at-and-t-authentication-api-openapi.yml
  format: yaml
  label: AT&T Authentication API
  slug: at-and-t-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-authentication-api-openapi.yml
- filename: at-and-t-balance-management-api-openapi.yml
  format: yaml
  label: AT&T Balance Management API
  slug: at-and-t-balance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-balance-management-api-openapi.yml
- filename: at-and-t-device-management-api-openapi.yml
  format: yaml
  label: AT&T Device Management API
  slug: at-and-t-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-device-management-api-openapi.yml
- filename: at-and-t-geographic-sites-api-openapi.yml
  format: yaml
  label: AT&T Geographic Sites API
  slug: at-and-t-geographic-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-geographic-sites-api-openapi.yml
- filename: at-and-t-inbox-management-api-openapi.yml
  format: yaml
  label: AT&T Inbox Management API
  slug: at-and-t-inbox-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-inbox-management-api-openapi.yml
- filename: at-and-t-messages-api-openapi.yml
  format: yaml
  label: AT&T Messages API
  slug: at-and-t-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-messages-api-openapi.yml
- filename: at-and-t-number-management-api-openapi.yml
  format: yaml
  label: AT&T Number Management API
  slug: at-and-t-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-number-management-api-openapi.yml
- filename: at-and-t-porting-api-openapi.yml
  format: yaml
  label: AT&T Porting API
  slug: at-and-t-porting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-porting-api-openapi.yml
- filename: at-and-t-product-orders-api-openapi.yml
  format: yaml
  label: AT&T Product Orders API
  slug: at-and-t-product-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-product-orders-api-openapi.yml
- filename: at-and-t-service-management-api-openapi.yml
  format: yaml
  label: AT&T Service Management API
  slug: at-and-t-service-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-service-management-api-openapi.yml
- filename: at-and-t-sms-messaging-api-openapi.yml
  format: yaml
  label: AT&T SMS Messaging API
  slug: at-and-t-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-sms-messaging-api-openapi.yml
- filename: at-and-t-subscriber-management-api-openapi.yml
  format: yaml
  label: AT&T Subscriber Management API
  slug: at-and-t-subscriber-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-subscriber-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: att.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.att.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: developer.att.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.att.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: At And T Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AT&T, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AT&T
provider_slug: at-and-t
slug: at-and-t-domain-security
source_filename: at-and-t-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.att.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: att.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/security/at-and-t-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
---
