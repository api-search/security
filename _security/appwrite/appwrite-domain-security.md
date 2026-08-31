---
api_specs:
- filename: appwrite-account-api-openapi.yml
  format: yaml
  label: Appwrite Account API
  slug: appwrite-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/openapi/appwrite-account-api-openapi.yml
- filename: appwrite-databases-api-openapi.yml
  format: yaml
  label: Appwrite Databases API
  slug: appwrite-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/openapi/appwrite-databases-api-openapi.yml
- filename: appwrite-storage-api-openapi.yml
  format: yaml
  label: Appwrite Storage API
  slug: appwrite-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/openapi/appwrite-storage-api-openapi.yml
- filename: appwrite-users-api-openapi.yml
  format: yaml
  label: Appwrite Users API
  slug: appwrite-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/openapi/appwrite-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appwrite.io
  spf: true
hosts:
- cert_expires: Sep 28 01:59:01 2026 GMT
  host: appwrite.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 19:03:11 2026 GMT
  host: cloud.appwrite.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appwrite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appwrite, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Appwrite
provider_slug: appwrite
slug: appwrite-domain-security
source_filename: appwrite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appwrite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 01:59:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.appwrite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:03:11 2026 GMT\n  hsts: false\ndomains:\n- domain: appwrite.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appwrite/refs/heads/main/security/appwrite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application
- Backends
- Mobile
- Open-Source
---
