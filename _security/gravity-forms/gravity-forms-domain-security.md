---
api_specs:
- filename: gravity-forms-openapi.yml
  format: yaml
  label: Gravity Forms REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravity-forms/refs/heads/main/openapi/gravity-forms-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gravityforms.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-wordpress-site.example
  spf: false
hosts:
- cert_expires: Oct  6 08:03:51 2026 GMT
  host: www.gravityforms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 08:03:51 2026 GMT
  host: docs.gravityforms.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
- host: your-wordpress-site.example
  https: false
kind: domain-security
layout: security
method: probed
name: Gravity Forms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gravity Forms, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gravity Forms
provider_slug: gravity-forms
slug: gravity-forms-domain-security
source_filename: gravity-forms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gravityforms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:03:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.gravityforms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:03:51 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: your-wordpress-site.example\n  https: false\ndomains:\n- domain: gravityforms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: your-wordpress-site.example\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravity-forms/refs/heads/main/security/gravity-forms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- WordPress
- Forms
- Form Builder
- Surveys
- Workflow
- Plugins
---
