---
api_specs:
- filename: noun-project-autocomplete-api-openapi.yml
  format: yaml
  label: Noun Project Autocomplete API
  slug: noun-project-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/openapi/noun-project-autocomplete-api-openapi.yml
- filename: noun-project-blocklist-api-openapi.yml
  format: yaml
  label: Noun Project Blocklist API
  slug: noun-project-blocklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/openapi/noun-project-blocklist-api-openapi.yml
- filename: noun-project-collection-api-openapi.yml
  format: yaml
  label: Noun Project Collection API
  slug: noun-project-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/openapi/noun-project-collection-api-openapi.yml
- filename: noun-project-icon-api-openapi.yml
  format: yaml
  label: Noun Project Icon API
  slug: noun-project-icon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/openapi/noun-project-icon-api-openapi.yml
- filename: noun-project-usage-api-openapi.yml
  format: yaml
  label: Noun Project Usage API
  slug: noun-project-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/openapi/noun-project-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thenounproject.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: thenounproject.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api.thenounproject.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Noun Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noun Project, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Noun Project
provider_slug: noun-project
slug: noun-project-domain-security
source_filename: noun-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thenounproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\n- host: api.thenounproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: thenounproject.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noun-project/refs/heads/main/security/noun-project-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Art And Design
- Icons
- SVG
- Visual Language
- Design Assets
- Public APIs
---
