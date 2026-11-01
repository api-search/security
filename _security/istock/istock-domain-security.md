---
api_specs:
- filename: istock-countries-api-openapi.yml
  format: yaml
  label: iStock Countries API
  slug: istock-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-countries-api-openapi.yml
- filename: istock-downloads-api-openapi.yml
  format: yaml
  label: iStock Downloads API
  slug: istock-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-downloads-api-openapi.yml
- filename: istock-images-api-openapi.yml
  format: yaml
  label: iStock Images API
  slug: istock-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-images-api-openapi.yml
- filename: istock-search-api-openapi.yml
  format: yaml
  label: iStock Search API
  slug: istock-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-search-api-openapi.yml
- filename: istock-videos-api-openapi.yml
  format: yaml
  label: iStock Videos API
  slug: istock-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-videos-api-openapi.yml
- filename: istock-affiliatesearch-api-openapi.yml
  format: yaml
  label: iStock Affiliate Search API
  slug: istock-affiliatesearch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-affiliatesearch-api-openapi.yml
- filename: istock-aigenerator-api-openapi.yml
  format: yaml
  label: iStock AI Generator API
  slug: istock-aigenerator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-aigenerator-api-openapi.yml
- filename: istock-artists-api-openapi.yml
  format: yaml
  label: iStock Artists API
  slug: istock-artists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-artists-api-openapi.yml
- filename: istock-assetchanges-api-openapi.yml
  format: yaml
  label: iStock Asset Changes API
  slug: istock-assetchanges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-assetchanges-api-openapi.yml
- filename: istock-assetlicensing-api-openapi.yml
  format: yaml
  label: iStock Asset Licensing API
  slug: istock-assetlicensing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-assetlicensing-api-openapi.yml
- filename: istock-boards-api-openapi.yml
  format: yaml
  label: iStock Boards API
  slug: istock-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-boards-api-openapi.yml
- filename: istock-collections-api-openapi.yml
  format: yaml
  label: iStock Collections API
  slug: istock-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-collections-api-openapi.yml
- filename: istock-customers-api-openapi.yml
  format: yaml
  label: iStock Customers API
  slug: istock-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-customers-api-openapi.yml
- filename: istock-events-api-openapi.yml
  format: yaml
  label: iStock Events API
  slug: istock-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-events-api-openapi.yml
- filename: istock-imagematch-api-openapi.yml
  format: yaml
  label: iStock Image Match API
  slug: istock-imagematch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-imagematch-api-openapi.yml
- filename: istock-orders-api-openapi.yml
  format: yaml
  label: iStock Orders API
  slug: istock-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-orders-api-openapi.yml
- filename: istock-products-api-openapi.yml
  format: yaml
  label: iStock Products API
  slug: istock-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-products-api-openapi.yml
- filename: istock-purchases-api-openapi.yml
  format: yaml
  label: iStock Purchases API
  slug: istock-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-purchases-api-openapi.yml
- filename: istock-usage-api-openapi.yml
  format: yaml
  label: iStock Usage API
  slug: istock-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/istock/openapi/istock-usage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:dnsadmins@gettyimages.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: istockphoto.com
  spf: true
- caa:
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:dnsadmins@gettyimages.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gettyimages.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.istockphoto.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.gettyimages.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Istock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iStock, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: iStock
provider_slug: istock
slug: istock-domain-security
source_filename: istock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.istockphoto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.gettyimages.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: istockphoto.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dnsadmins@gettyimages.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gettyimages.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:dnsadmins@gettyimages.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://artifacts.apis.io/istock/security/istock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stock Media
- Image
- Video
- Illustrations
- Royalty-Free
- Getty
---
