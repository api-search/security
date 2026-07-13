---
api_specs:
- filename: datocms-content-management-api.yml
  format: yaml
  label: DatoCMS Content Management API
  slug: datocms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/openapi/datocms-content-management-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datocms.com
  spf: true
hosts:
- cert_expires: Aug 18 02:02:41 2026 GMT
  host: www.datocms.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 07:29:44 2026 GMT
  host: site-api.datocms.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 07:29:44 2026 GMT
  host: graphql.datocms.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datocms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DatoCMS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DatoCMS
provider_slug: datocms
slug: datocms-domain-security
source_filename: datocms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datocms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 02:02:41 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: site-api.datocms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:29:44 2026 GMT\n  hsts: null\n- host: graphql.datocms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:29:44 2026 GMT\n  hsts: null\ndomains:\n- domain: datocms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datocms/refs/heads/main/security/datocms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Delivery
- Content Management
- GraphQL
- Headless CMS
---
