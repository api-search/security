---
api_specs:
- filename: intralinks-authentication-api-openapi.yml
  format: yaml
  label: Intralinks Authentication API
  slug: intralinks-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-authentication-api-openapi.yml
- filename: intralinks-custom-fields-api-openapi.yml
  format: yaml
  label: Intralinks Custom Fields API
  slug: intralinks-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-custom-fields-api-openapi.yml
- filename: intralinks-documents-api-openapi.yml
  format: yaml
  label: Intralinks Documents API
  slug: intralinks-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-documents-api-openapi.yml
- filename: intralinks-folders-api-openapi.yml
  format: yaml
  label: Intralinks Folders API
  slug: intralinks-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-folders-api-openapi.yml
- filename: intralinks-groups-api-openapi.yml
  format: yaml
  label: Intralinks Groups API
  slug: intralinks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-groups-api-openapi.yml
- filename: intralinks-permissions-api-openapi.yml
  format: yaml
  label: Intralinks Permissions API
  slug: intralinks-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-permissions-api-openapi.yml
- filename: intralinks-splash-api-openapi.yml
  format: yaml
  label: Intralinks Splash API
  slug: intralinks-splash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-splash-api-openapi.yml
- filename: intralinks-workspaces-api-openapi.yml
  format: yaml
  label: Intralinks Workspaces API
  slug: intralinks-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/openapi/intralinks-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: intralinks.com
  spf: true
hosts:
- host: developers.intralinks.com
  https: false
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.intralinks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intralinks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intralinks, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Intralinks
provider_slug: intralinks
slug: intralinks-domain-security
source_filename: intralinks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.intralinks.com\n  https: false\n- host: api.intralinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: intralinks.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intralinks/refs/heads/main/security/intralinks-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Document-Management
- Secure File Sharing
- Virtual Data Room
---
