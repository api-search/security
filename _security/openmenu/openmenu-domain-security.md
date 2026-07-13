---
api_specs:
- filename: openmenu-openapi.yml
  format: yaml
  label: OpenMenu API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmenu/refs/heads/main/openapi/openmenu-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openmenu.com
  spf: false
hosts:
- cert_expires: Sep  6 23:03:34 2026 GMT
  host: openmenu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 23:03:34 2026 GMT
  host: www.openmenu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openmenu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenMenu, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: OpenMenu
provider_slug: openmenu
slug: openmenu-domain-security
source_filename: openmenu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openmenu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:03:34 2026 GMT\n  hsts: null\n- host: www.openmenu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:03:34 2026 GMT\n  hsts: null\ndomains:\n- domain: openmenu.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmenu/refs/heads/main/security/openmenu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Restaurant
- Menus
- Menu Data
- Search
- Nutrition
- Structured Data
---
