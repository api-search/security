---
api_specs:
- filename: microsoft-onedrive-drives-drive-actions-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.drive.Actions API
  slug: microsoft-onedrive-drives-drive-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-drive-actions-api-openapi.yml
- filename: microsoft-onedrive-drives-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.drive API
  slug: microsoft-onedrive-drives-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-drive-api-openapi.yml
- filename: microsoft-onedrive-drives-drive-functions-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.drive.Functions API
  slug: microsoft-onedrive-drives-drive-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-drive-functions-api-openapi.yml
- filename: microsoft-onedrive-drives-driveitem-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.drive Item API
  slug: microsoft-onedrive-drives-driveitem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-driveitem-api-openapi.yml
- filename: microsoft-onedrive-drives-list-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.list API
  slug: microsoft-onedrive-drives-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-list-api-openapi.yml
- filename: microsoft-onedrive-drives-user-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.user API
  slug: microsoft-onedrive-drives-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-user-api-openapi.yml
- filename: microsoft-onedrive-groups-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Groups.drive API
  slug: microsoft-onedrive-groups-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-groups-drive-api-openapi.yml
- filename: microsoft-onedrive-groups-site-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Groups.site API
  slug: microsoft-onedrive-groups-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-groups-site-api-openapi.yml
- filename: microsoft-onedrive-me-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Me.drive API
  slug: microsoft-onedrive-me-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-me-drive-api-openapi.yml
- filename: microsoft-onedrive-sites-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Sites.drive API
  slug: microsoft-onedrive-sites-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-sites-drive-api-openapi.yml
- filename: microsoft-onedrive-users-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Users.drive API
  slug: microsoft-onedrive-users-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-users-drive-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft OneDrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft OneDrive, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft OneDrive
provider_slug: microsoft-onedrive
slug: microsoft-onedrive-domain-security
source_filename: microsoft-onedrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-onedrive/security/microsoft-onedrive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Storage
- File Storage
- File
- Microsoft
- Microsoft 365
---
