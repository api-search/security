---
api_specs:
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Menu / Catalog API
  slug: menu-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Stores API
  slug: stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Stock / Availability API
  slug: stock-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
- filename: petpooja-openapi.yml
  format: yaml
  label: Petpooja Callbacks API
  slug: callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/openapi/petpooja-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: petpooja.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: www.petpooja.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: onlineorderingapisv210.docs.apiary.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: qle1yy2ydc.execute-api.ap-southeast-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Petpooja Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Petpooja, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Petpooja
provider_slug: petpooja
slug: petpooja-domain-security
source_filename: petpooja-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.petpooja.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: onlineorderingapisv210.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: qle1yy2ydc.execute-api.ap-southeast-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: petpooja.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petpooja/refs/heads/main/security/petpooja-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- POS
- Online Ordering
- Menu
- Food Delivery
---
