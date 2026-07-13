---
api_specs:
- filename: softwareone-openapi.yml
  format: yaml
  label: SoftwareOne Marketplace Platform API
  slug: marketplace-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/softwareone/refs/heads/main/openapi/softwareone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: softwareone.com
  spf: true
hosts:
- cert_expires: Aug 13 18:29:56 2026 GMT
  host: www.softwareone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 08:58:57 2026 GMT
  host: docs.platform.softwareone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.platform.softwareone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Softwareone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoftwareOne, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SoftwareOne
provider_slug: softwareone
slug: softwareone-domain-security
source_filename: softwareone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.softwareone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 18:29:56 2026 GMT\n  hsts: null\n- host: docs.platform.softwareone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:58:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.platform.softwareone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: softwareone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/softwareone/refs/heads/main/security/softwareone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- Software Procurement
- Cloud Management
- License Management
- SaaS
---
