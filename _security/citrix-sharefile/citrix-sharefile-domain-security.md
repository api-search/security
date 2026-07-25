---
api_specs:
- filename: citrix-sharefile-accounts-api-openapi.yml
  format: yaml
  label: Citrix ShareFile Accounts API
  slug: citrix-sharefile-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/openapi/citrix-sharefile-accounts-api-openapi.yml
- filename: citrix-sharefile-groups-api-openapi.yml
  format: yaml
  label: Citrix ShareFile Groups API
  slug: citrix-sharefile-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/openapi/citrix-sharefile-groups-api-openapi.yml
- filename: citrix-sharefile-items-api-openapi.yml
  format: yaml
  label: Citrix ShareFile Items API
  slug: citrix-sharefile-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/openapi/citrix-sharefile-items-api-openapi.yml
- filename: citrix-sharefile-sessions-api-openapi.yml
  format: yaml
  label: Citrix ShareFile Sessions API
  slug: citrix-sharefile-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/openapi/citrix-sharefile-sessions-api-openapi.yml
- filename: citrix-sharefile-shares-api-openapi.yml
  format: yaml
  label: Citrix ShareFile Shares API
  slug: citrix-sharefile-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/openapi/citrix-sharefile-shares-api-openapi.yml
- filename: citrix-sharefile-users-api-openapi.yml
  format: yaml
  label: Citrix ShareFile Users API
  slug: citrix-sharefile-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/openapi/citrix-sharefile-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sharefile.com
  spf: true
hosts:
- cert_expires: Oct  6 19:32:53 2026 GMT
  host: www.sharefile.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: api.sharefile.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Citrix Sharefile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citrix ShareFile, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Citrix ShareFile
provider_slug: citrix-sharefile
slug: citrix-sharefile-domain-security
source_filename: citrix-sharefile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sharefile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:32:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sharefile.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sharefile.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citrix-sharefile/refs/heads/main/security/citrix-sharefile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- File Sharing
- Document Workflow
- Secure File Transfer
- E-Signature
- Client Portal
- Content Collaboration
---
