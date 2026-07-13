---
api_specs:
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Clients API
  slug: repsly-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Representatives API
  slug: repsly-representatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Visits API
  slug: repsly-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Products API
  slug: repsly-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Forms API
  slug: repsly-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Photos API
  slug: repsly-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Pricelists API
  slug: repsly-pricelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Purchase Orders API
  slug: repsly-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
- filename: repsly-openapi.yml
  format: yaml
  label: Repsly Import and Export API
  slug: repsly-import-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/openapi/repsly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: repsly.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 16 11:10:09 2026 GMT
  host: www.repsly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: repsly-dev.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api.repsly.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Repsly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Repsly, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Repsly
provider_slug: repsly
slug: repsly-domain-security
source_filename: repsly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.repsly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 11:10:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: repsly-dev.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.repsly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: repsly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/repsly/refs/heads/main/security/repsly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail Execution
- Field Sales
- Merchandising
- CPG
- Retail Audits
- Sales Force Automation
---
