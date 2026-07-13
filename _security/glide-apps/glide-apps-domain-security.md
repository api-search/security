---
api_specs:
- filename: glide-apps-openapi.yml
  format: yaml
  label: Glide Tables API
  slug: glide-apps-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/openapi/glide-apps-openapi.yml
- filename: glide-apps-openapi.yml
  format: yaml
  label: Glide Big Tables Rows API
  slug: glide-apps-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/openapi/glide-apps-openapi.yml
- filename: glide-apps-openapi.yml
  format: yaml
  label: Glide Stash & Bulk API
  slug: glide-apps-stash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/openapi/glide-apps-openapi.yml
- filename: glide-apps-openapi.yml
  format: yaml
  label: Glide Queries API
  slug: glide-apps-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/openapi/glide-apps-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: glideapps.com
  spf: true
hosts:
- cert_expires: Aug 13 07:54:37 2026 GMT
  host: www.glideapps.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:54:55 2026 GMT
  host: apidocs.glideapps.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:26:23 2026 GMT
  host: api.glideapps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glide Apps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glide, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Glide
provider_slug: glide-apps
slug: glide-apps-domain-security
source_filename: glide-apps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glideapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 07:54:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.glideapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:54:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.glideapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:26:23 2026 GMT\n  hsts: null\ndomains:\n- domain: glideapps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glide-apps/refs/heads/main/security/glide-apps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- No Code
- App Builder
- Tables
- Big Tables
- Data
- AI
---
