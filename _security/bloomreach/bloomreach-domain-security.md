---
api_specs:
- filename: search-category.yaml
  format: yaml
  label: Bloomreach Discovery API
  slug: bloomreach-discovery-api
  spec_type: OpenAPI
  url: https://github.com/bloomreach/api-specs/blob/main/discovery/search-category.yaml
- filename: catalog-management.yaml
  format: yaml
  label: Bloomreach Discovery Catalog Management API
  slug: bloomreach-discovery-catalog-management-api
  spec_type: OpenAPI
  url: https://github.com/bloomreach/api-specs/blob/main/discovery/catalog-management.yaml
- filename: workspace-import-api.yaml
  format: yaml
  label: Bloomreach Data Hub Workspace Import API
  slug: bloomreach-data-hub-workspace-import-api
  spec_type: OpenAPI
  url: https://github.com/bloomreach/api-specs/blob/main/data-hub/workspace-import-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bloomreach.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: dxpapi.com
  spf: false
hosts:
- cert_expires: Oct  1 23:48:11 2026 GMT
  host: www.bloomreach.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:52:17 2026 GMT
  host: documentation.bloomreach.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 20:25:23 2026 GMT
  host: core.dxpapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomreach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomreach, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bloomreach
provider_slug: bloomreach
slug: bloomreach-domain-security
source_filename: bloomreach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bloomreach.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:48:11 2026 GMT\n  hsts: false\n- host: documentation.bloomreach.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:52:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: core.dxpapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:25:23 2026 GMT\n  hsts: null\ndomains:\n- domain: bloomreach.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dxpapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomreach/refs/heads/main/security/bloomreach-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Commerce
- Search
- Merchandising
- Recommendations
- Customer Data Platform
- CDP
- Email Marketing
- SMS Marketing
- Marketing Automation
- Headless CMS
- Personalization
- E-commerce
---
