---
api_specs:
- filename: filen-health-api-openapi.yml
  format: yaml
  label: Filen Health API
  slug: filen-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-health-api-openapi.yml
- filename: filen-items-api-openapi.yml
  format: yaml
  label: Filen Items API
  slug: filen-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-items-api-openapi.yml
- filename: filen-items-directories-api-openapi.yml
  format: yaml
  label: 'Filen Items: Directories API'
  slug: filen-items-directories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-items-directories-api-openapi.yml
- filename: filen-items-files-api-openapi.yml
  format: yaml
  label: 'Filen Items: Files API'
  slug: filen-items-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-items-files-api-openapi.yml
- filename: filen-public-links-api-openapi.yml
  format: yaml
  label: Filen Public Links API
  slug: filen-public-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-public-links-api-openapi.yml
- filename: filen-shared-api-openapi.yml
  format: yaml
  label: Filen Shared API
  slug: filen-shared-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-shared-api-openapi.yml
- filename: filen-user-api-openapi.yml
  format: yaml
  label: Filen User API
  slug: filen-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filen/openapi/filen-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: filen.io
  spf: true
hosts:
- cert_expires: Dec 10 14:19:03 2026 GMT
  host: filen.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Filen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Filen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Filen
provider_slug: filen
slug: filen-domain-security
source_filename: filen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filen.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 14:19:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: filen.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/filen/security/filen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Storage
- Encryption
- Zero Knowledge
- File Sync
---
