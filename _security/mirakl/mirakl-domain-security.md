---
api_specs:
- filename: mirakl-mmp-seller-openapi.json
  format: json
  label: Mirakl Marketplace Platform — Seller API
  slug: mirakl-marketplace-platform-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mmp-seller-openapi.json
- filename: mirakl-mmp-operator-openapi.json
  format: json
  label: Mirakl Marketplace Platform — Operator API
  slug: mirakl-marketplace-platform-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mmp-operator-openapi.json
- filename: mirakl-mms-seller-openapi.json
  format: json
  label: Mirakl Platform for Services — Seller API
  slug: mirakl-platform-for-services-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mms-seller-openapi.json
- filename: mirakl-mms-operator-openapi.json
  format: json
  label: Mirakl Platform for Services — Operator API
  slug: mirakl-platform-for-services-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mms-operator-openapi.json
- filename: mirakl-mcm-seller-openapi.json
  format: json
  label: Mirakl Catalog Manager — Seller API
  slug: mirakl-catalog-manager-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mcm-seller-openapi.json
- filename: mirakl-mcm-operator-openapi.json
  format: json
  label: Mirakl Catalog Manager — Operator API
  slug: mirakl-catalog-manager-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-mcm-operator-openapi.json
- filename: mirakl-connect-channel-openapi.json
  format: json
  label: Mirakl Connect Channel Platform API
  slug: mirakl-connect-channel-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/openapi/mirakl-connect-channel-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mirakl.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mirakl.net
  spf: true
hosts:
- cert_expires: Oct 12 15:38:23 2026 GMT
  host: www.mirakl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-instance.mirakl.net
  https: false
kind: domain-security
layout: security
method: probed
name: Mirakl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirakl, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mirakl
provider_slug: mirakl
slug: mirakl-domain-security
source_filename: mirakl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mirakl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:38:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-instance.mirakl.net\n  https: false\ndomains:\n- domain: mirakl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mirakl.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirakl/refs/heads/main/security/mirakl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Commerce
- eCommerce
- Marketplace
- Dropship
- Retail
- Catalog
- Orders
- Retail Media
- B2B
---
