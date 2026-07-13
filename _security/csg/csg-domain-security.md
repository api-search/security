---
api_specs:
- filename: csg-forte-rest-openapi.yml
  format: yaml
  label: CSG Forte REST API
  slug: csg-forte-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/csg/refs/heads/main/openapi/csg-forte-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: csgi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forte.net
  spf: true
hosts:
- cert_expires: Sep 28 07:00:46 2026 GMT
  host: www.csgi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:51:51 2026 GMT
  host: www.forte.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 10:27:36 2026 GMT
  host: developers.forte.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Csg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CSG Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CSG Systems
provider_slug: csg
slug: csg-domain-security
source_filename: csg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.csgi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:00:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.forte.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:51:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.forte.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:27:36 2026 GMT\n  hsts: false\ndomains:\n- domain: csgi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: forte.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/csg/refs/heads/main/security/csg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Customer Engagement
- Payments
- Revenue Management
- Telecom
---
