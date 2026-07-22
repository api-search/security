---
api_specs:
- filename: propelplm-core-openapi.yml
  format: yaml
  label: Propel PLM Core REST API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-core-openapi.yml
- filename: propelplm-pim-openapi.yml
  format: yaml
  label: Propel PIM API
  slug: pim
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelplm/refs/heads/main/openapi/propelplm-pim-openapi.yml
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
