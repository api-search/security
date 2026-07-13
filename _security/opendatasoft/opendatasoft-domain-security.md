---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Opendatasoft Explore API v2.1
  slug: opendatasoft-explore-api-v21
  spec_type: OpenAPI
  url: https://public.opendatasoft.com/api/explore/v2.1/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: huwise.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opendatasoft.com
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: www.huwise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 22:20:55 2026 GMT
  host: help.opendatasoft.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 08:40:08 2026 GMT
  host: public.opendatasoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendatasoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opendatasoft, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Opendatasoft
provider_slug: opendatasoft
slug: opendatasoft-domain-security
source_filename: opendatasoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huwise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.opendatasoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:20:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public.opendatasoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 08:40:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: huwise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: opendatasoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendatasoft/refs/heads/main/security/opendatasoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- Datasets
- Public Data
- OData
- REST
- Government
- Cities
---
