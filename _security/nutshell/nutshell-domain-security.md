---
api_specs:
- filename: nutshell-openapi.yml
  format: yaml
  label: Nutshell REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutshell/refs/heads/main/openapi/nutshell-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nutshell.com
  spf: true
hosts:
- cert_expires: Aug 18 22:46:36 2026 GMT
  host: www.nutshell.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 16:13:17 2026 GMT
  host: developers.nutshell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: app.nutshell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nutshell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nutshell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nutshell
provider_slug: nutshell
slug: nutshell-domain-security
source_filename: nutshell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nutshell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 22:46:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.nutshell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 16:13:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.nutshell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nutshell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutshell/refs/heads/main/security/nutshell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Sales
- Pipeline Management
- Email Marketing
- Contact Management
- Sales Automation
---
