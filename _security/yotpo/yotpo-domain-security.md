---
api_specs:
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Reviews & Ratings API
  slug: yotpo-reviews-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Loyalty & Referrals API
  slug: yotpo-loyalty-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo SMS & Email API
  slug: yotpo-sms-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo UGC & Visual API
  slug: yotpo-ugc-visual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Subscriptions API
  slug: yotpo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
- filename: yotpo-openapi.yml
  format: yaml
  label: Yotpo Webhooks
  slug: yotpo-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/openapi/yotpo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yotpo.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.yotpo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 14:37:29 2026 GMT
  host: apidocs.yotpo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api.yotpo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yotpo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yotpo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yotpo
provider_slug: yotpo
slug: yotpo-domain-security
source_filename: yotpo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yotpo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.yotpo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:37:29 2026 GMT\n  hsts: null\n- host: api.yotpo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: yotpo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yotpo/refs/heads/main/security/yotpo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eCommerce
- Reviews
- Loyalty
- Retention Marketing
- UGC
---
