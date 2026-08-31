---
api_specs:
- filename: wallapop-categories-api-openapi.yml
  format: yaml
  label: Wallapop Categories API
  slug: wallapop-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-categories-api-openapi.yml
- filename: wallapop-delivery-api-openapi.yml
  format: yaml
  label: Wallapop Delivery API
  slug: wallapop-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-delivery-api-openapi.yml
- filename: wallapop-disputes-api-openapi.yml
  format: yaml
  label: Wallapop Disputes API
  slug: wallapop-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-disputes-api-openapi.yml
- filename: wallapop-items-api-openapi.yml
  format: yaml
  label: Wallapop Items API
  slug: wallapop-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-items-api-openapi.yml
- filename: wallapop-transactions-api-openapi.yml
  format: yaml
  label: Wallapop Transactions API
  slug: wallapop-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-transactions-api-openapi.yml
- filename: wallapop-webhooks-api-openapi.yml
  format: yaml
  label: Wallapop Webhooks API
  slug: wallapop-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/openapi/wallapop-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wallapop.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.wallapop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: connect.wallapop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wallapop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wallapop, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wallapop
provider_slug: wallapop
slug: wallapop-domain-security
source_filename: wallapop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wallapop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.wallapop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wallapop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallapop/refs/heads/main/security/wallapop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Marketplace
- E-Commerce
- Second-Hand
- Classifieds
- Shipping
- Webhook
---
