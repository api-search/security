---
api_specs:
- filename: loudcrowd-attribution-events-api-api-openapi.yml
  format: yaml
  label: LoudCrowd Attribution Events API
  slug: loudcrowd-attribution-events-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-attribution-events-api-api-openapi.yml
- filename: loudcrowd-brand-api-api-openapi.yml
  format: yaml
  label: LoudCrowd Brand API
  slug: loudcrowd-brand-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-brand-api-api-openapi.yml
- filename: loudcrowd-product-data-api-openapi.yml
  format: yaml
  label: LoudCrowd Product Data API
  slug: loudcrowd-product-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-product-data-api-openapi.yml
- filename: loudcrowd-storefrontambassador-api-openapi.yml
  format: yaml
  label: LoudCrowd Storefront Ambassador API
  slug: loudcrowd-storefrontambassador-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-storefrontambassador-api-openapi.yml
- filename: loudcrowd-storefrontcollections-api-openapi.yml
  format: yaml
  label: LoudCrowd Storefront Collections API
  slug: loudcrowd-storefrontcollections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-storefrontcollections-api-openapi.yml
- filename: loudcrowd-storefrontfeeditems-api-openapi.yml
  format: yaml
  label: LoudCrowd Storefront Feed Items API
  slug: loudcrowd-storefrontfeeditems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-storefrontfeeditems-api-openapi.yml
- filename: loudcrowd-storefrontmediadetails-api-openapi.yml
  format: yaml
  label: LoudCrowd Storefront Media Details API
  slug: loudcrowd-storefrontmediadetails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-storefrontmediadetails-api-openapi.yml
- filename: loudcrowd-storefrontproductdetails-api-openapi.yml
  format: yaml
  label: LoudCrowd Storefront Product Details API
  slug: loudcrowd-storefrontproductdetails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/openapi/loudcrowd-storefrontproductdetails-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: loudcrowd.com
  spf: true
hosts:
- cert_expires: Oct 28 21:19:15 2026 GMT
  host: loudcrowd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 18:22:01 2026 GMT
  host: docs.loudcrowd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api.loudcrowd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loudcrowd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LoudCrowd, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LoudCrowd
provider_slug: loudcrowd
slug: loudcrowd-domain-security
source_filename: loudcrowd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loudcrowd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 21:19:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.loudcrowd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 18:22:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.loudcrowd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: loudcrowd.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loudcrowd/refs/heads/main/security/loudcrowd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Creator Marketing
- Influencer Marketing
- Affiliate Marketing
- Ecommerce
- Creator Commerce
- Attribution
- Social Commerce
- Shopify
- User Generated Content
- Commissions
- Retail
- Marketing
---
