---
api_specs:
- filename: amazon-ad-groups-api-openapi.yml
  format: yaml
  label: Amazon Ad Groups API
  slug: amazon-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-ad-groups-api-openapi.yml
- filename: amazon-campaigns-api-openapi.yml
  format: yaml
  label: Amazon Campaigns API
  slug: amazon-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-campaigns-api-openapi.yml
- filename: amazon-catalog-api-openapi.yml
  format: yaml
  label: Amazon Catalog API
  slug: amazon-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-catalog-api-openapi.yml
- filename: amazon-charge-permissions-api-openapi.yml
  format: yaml
  label: Amazon Charge Permissions API
  slug: amazon-charge-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-charge-permissions-api-openapi.yml
- filename: amazon-charges-api-openapi.yml
  format: yaml
  label: Amazon Charges API
  slug: amazon-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-charges-api-openapi.yml
- filename: amazon-checkout-sessions-api-openapi.yml
  format: yaml
  label: Amazon Checkout Sessions API
  slug: amazon-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-checkout-sessions-api-openapi.yml
- filename: amazon-finances-api-openapi.yml
  format: yaml
  label: Amazon Finances API
  slug: amazon-finances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-finances-api-openapi.yml
- filename: amazon-inventory-api-openapi.yml
  format: yaml
  label: Amazon Inventory API
  slug: amazon-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-inventory-api-openapi.yml
- filename: amazon-keywords-api-openapi.yml
  format: yaml
  label: Amazon Keywords API
  slug: amazon-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-keywords-api-openapi.yml
- filename: amazon-listings-api-openapi.yml
  format: yaml
  label: Amazon Listings API
  slug: amazon-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-listings-api-openapi.yml
- filename: amazon-orders-api-openapi.yml
  format: yaml
  label: Amazon Orders API
  slug: amazon-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-orders-api-openapi.yml
- filename: amazon-profiles-api-openapi.yml
  format: yaml
  label: Amazon Profiles API
  slug: amazon-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-profiles-api-openapi.yml
- filename: amazon-refunds-api-openapi.yml
  format: yaml
  label: Amazon Refunds API
  slug: amazon-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-refunds-api-openapi.yml
- filename: amazon-reports-api-openapi.yml
  format: yaml
  label: Amazon Reports API
  slug: amazon-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-reports-api-openapi.yml
- filename: amazon-targets-api-openapi.yml
  format: yaml
  label: Amazon Targets API
  slug: amazon-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/openapi/amazon-targets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: developer.amazon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.amazon.com
  hsts: true
  hsts_max_age: 47474747
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: developer-docs.amazon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon
provider_slug: amazon
slug: amazon-domain-security
source_filename: amazon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47474747\n- host: developer-docs.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon/refs/heads/main/security/amazon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon
- Advertising
- Alexa
- E-Commerce
- Marketplace
- Payments
- Voice
- Fortune 100
---
