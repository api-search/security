---
api_specs:
- filename: ikea-product-catalog-openapi.yml
  format: yaml
  label: IKEA Product Catalog API (Unofficial)
  slug: product-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-product-catalog-openapi.yml
- filename: ikea-search-openapi.yml
  format: yaml
  label: IKEA Search API (Unofficial)
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-search-openapi.yml
- filename: ikea-sales-item-openapi.yml
  format: yaml
  label: IKEA Sales Item API (Unofficial)
  slug: sales-item
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-sales-item-openapi.yml
- filename: ikea-after-purchase-ordering-openapi.yml
  format: yaml
  label: IKEA After Purchase Ordering API (Unofficial)
  slug: after-purchase-ordering
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ikea/main/openapi/ikea-after-purchase-ordering-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:caa@inter.IKEA.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ikea.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ingka.com
  spf: true
hosts:
- cert_expires: Oct  3 14:53:21 2026 GMT
  host: www.ikea.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 15:45:21 2026 GMT
  host: api.salesitem.ingka.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 18:14:19 2026 GMT
  host: api.prod.apo.ingka.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ikea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IKEA, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IKEA
provider_slug: ikea
slug: ikea-domain-security
source_filename: ikea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ikea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:53:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.salesitem.ingka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 15:45:21 2026 GMT\n  hsts: null\n- host: api.prod.apo.ingka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:14:19 2026 GMT\n  hsts: null\ndomains:\n- domain: ikea.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:caa@inter.IKEA.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ingka.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\
  \n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikea/refs/heads/main/security/ikea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Retail
- Home Furnishings
- Consumer Products
- Opensource
- Community
- Unofficial API
- Smart Home
---
