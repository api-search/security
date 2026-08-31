---
api_specs:
- filename: propelplm-assets-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) assets API
  slug: propelplm-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-assets-api-openapi.yml
- filename: propelplm-attachment-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Attachment API
  slug: propelplm-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-attachment-api-openapi.yml
- filename: propelplm-bill-of-material-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Bill of Material API
  slug: propelplm-bill-of-material-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-bill-of-material-api-openapi.yml
- filename: propelplm-bom-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) BOM API
  slug: propelplm-bom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-bom-api-openapi.yml
- filename: propelplm-categories-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) categories API
  slug: propelplm-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-categories-api-openapi.yml
- filename: propelplm-change-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) change API
  slug: propelplm-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-change-api-openapi.yml
- filename: propelplm-channels-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) channels API
  slug: propelplm-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-channels-api-openapi.yml
- filename: propelplm-configuration-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Configuration API
  slug: propelplm-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-configuration-api-openapi.yml
- filename: propelplm-item-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) Item API
  slug: propelplm-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-item-api-openapi.yml
- filename: propelplm-manufactureritem-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) ManufacturerItem API
  slug: propelplm-manufactureritem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-manufactureritem-api-openapi.yml
- filename: propelplm-manufacturerpart-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) ManufacturerPart API
  slug: propelplm-manufacturerpart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-manufacturerpart-api-openapi.yml
- filename: propelplm-markup-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) markup API
  slug: propelplm-markup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-markup-api-openapi.yml
- filename: propelplm-products-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) products API
  slug: propelplm-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-products-api-openapi.yml
- filename: propelplm-variants-api-openapi.yml
  format: yaml
  label: Propel Software (Propel PLM) variants API
  slug: propelplm-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-variants-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: propelsoftware.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: propelplm.com
  spf: true
hosts:
- cert_expires: Oct 16 14:43:07 2026 GMT
  host: www.propelsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 08:52:18 2026 GMT
  host: developer.propelplm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: na85.salesforce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propelplm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Propel Software (Propel PLM), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Propel Software (Propel PLM)
provider_slug: propelplm
slug: propelplm-domain-security
source_filename: propelplm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propelsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.propelplm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:52:18 2026 GMT\n  hsts: false\n- host: na85.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: propelsoftware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: propelplm.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/security/propelplm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Product Lifecycle Management
- PLM
- Quality Management
- QMS
- Product Information Management
- PIM
- Manufacturing
- Salesforce
- Bill of Materials
- Change Management
---
