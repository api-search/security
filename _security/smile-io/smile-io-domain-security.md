---
api_specs:
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Customers API
  slug: smile-io-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Points Transactions API
  slug: smile-io-points-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Points Products API
  slug: smile-io-points-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Reward Fulfillments API
  slug: smile-io-rewards-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Earning Rules API
  slug: smile-io-earning-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io VIP Tiers API
  slug: smile-io-vip-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
- filename: smile-io-openapi.yml
  format: yaml
  label: Smile.io Activities API
  slug: smile-io-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/openapi/smile-io-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@smile.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smile.io
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: smile.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:17:31 2026 GMT
  host: dev.smile.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: api.smile.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smile Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smile.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smile.io
provider_slug: smile-io
slug: smile-io-domain-security
source_filename: smile-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smile.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.smile.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:17:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.smile.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: smile.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@smile.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smile-io/refs/heads/main/security/smile-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Rewards
- Referrals
- E-commerce
- Points
- Customer Retention
- Shopify
---
