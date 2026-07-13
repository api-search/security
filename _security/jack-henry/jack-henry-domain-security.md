---
api_specs:
- filename: banno-consumer-api-openapi.yml
  format: yaml
  label: Banno Consumer API
  slug: banno-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-consumer-api-openapi.yml
- filename: banno-admin-api-openapi.yml
  format: yaml
  label: Banno Admin API
  slug: banno-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-admin-api-openapi.yml
- filename: banno-plugin-framework-openapi.yml
  format: yaml
  label: Banno Plugin Framework
  slug: banno-plugin-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-plugin-framework-openapi.yml
- filename: banno-authentication-framework-openapi.yml
  format: yaml
  label: Banno Authentication Framework
  slug: banno-authentication-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/banno-authentication-framework-openapi.yml
- filename: jxchange-rest-openapi.yml
  format: yaml
  label: jXchange REST
  slug: jxchange-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/jxchange-rest-openapi.yml
- filename: jack-henry-payments-openapi.yml
  format: yaml
  label: Jack Henry Payments
  slug: jack-henry-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/openapi/jack-henry-payments-openapi.yml
- filename: enterprise-event-system-asyncapi.yml
  format: yaml
  label: Enterprise Event System
  slug: enterprise-event-system
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/asyncapi/enterprise-event-system-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jackhenry.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: jackhenry.dev
  spf: false
hosts:
- cert_expires: Sep 16 01:03:39 2026 GMT
  host: www.jackhenry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 11:46:25 2026 GMT
  host: jackhenry.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.banno.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Jack Henry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jack Henry & Associates, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jack Henry & Associates
provider_slug: jack-henry
slug: jack-henry-domain-security
source_filename: jack-henry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jackhenry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:03:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jackhenry.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:46:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.banno.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: jackhenry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jackhenry.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jack-henry/refs/heads/main/security/jack-henry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Core Banking
- Digital Banking
- Payments
- Lending
- Fraud
- Open Banking
- Community Banks
- Credit Unions
- Fintech
- OAuth
- OpenID Connect
---
