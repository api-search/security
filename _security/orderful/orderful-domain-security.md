---
api_specs:
- filename: orderful-conversion-api-openapi.yml
  format: yaml
  label: Orderful Conversion API
  slug: orderful-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-conversion-api-openapi.yml
- filename: orderful-delivery-api-openapi.yml
  format: yaml
  label: Orderful Delivery API
  slug: orderful-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-delivery-api-openapi.yml
- filename: orderful-inbox-api-openapi.yml
  format: yaml
  label: Orderful Inbox API
  slug: orderful-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-inbox-api-openapi.yml
- filename: orderful-label-api-openapi.yml
  format: yaml
  label: Orderful Label API
  slug: orderful-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-label-api-openapi.yml
- filename: orderful-organization-api-openapi.yml
  format: yaml
  label: Orderful Organization API
  slug: orderful-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-organization-api-openapi.yml
- filename: orderful-poller-api-openapi.yml
  format: yaml
  label: Orderful Poller API
  slug: orderful-poller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-poller-api-openapi.yml
- filename: orderful-relationship-api-openapi.yml
  format: yaml
  label: Orderful Relationship API
  slug: orderful-relationship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-relationship-api-openapi.yml
- filename: orderful-transaction-api-openapi.yml
  format: yaml
  label: Orderful Transaction API
  slug: orderful-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-transaction-api-openapi.yml
- filename: orderful-transaction-v3-api-openapi.yml
  format: yaml
  label: Orderful Transaction (v3) API
  slug: orderful-transaction-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/openapi/orderful-transaction-v3-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@orderful.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: orderful.com
  spf: true
hosts:
- cert_expires: Sep 19 22:10:46 2026 GMT
  host: orderful.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orderful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orderful, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Orderful
provider_slug: orderful
slug: orderful-domain-security
source_filename: orderful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orderful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:10:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orderful.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@orderful.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderful/refs/heads/main/security/orderful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- EDI
- Electronic Data Interchange
- Supply Chain
- B2B
- Logistics
- Retail
- Transaction
- Integration
---
