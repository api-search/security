---
api_specs:
- filename: holded-openapi.yml
  format: yaml
  label: Holded REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/openapi/holded-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: holded.com
  spf: true
hosts:
- cert_expires: Aug 17 13:49:06 2026 GMT
  host: www.holded.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 25 16:44:06 2026 GMT
  host: developers.holded.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: api.holded.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holded Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Holded, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Holded
provider_slug: holded
slug: holded-domain-security
source_filename: holded-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.holded.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 13:49:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.holded.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 25 16:44:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.holded.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: holded.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/security/holded-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- CRM
- Accounting
- Invoicing
- Business Management
- SMB
- Spain
---
