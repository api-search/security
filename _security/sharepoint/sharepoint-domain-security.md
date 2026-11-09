---
api_specs:
- filename: sharepoint-files-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Files API
  slug: sharepoint-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-files-api-openapi.yml
- filename: sharepoint-items-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Items API
  slug: sharepoint-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-items-api-openapi.yml
- filename: sharepoint-lists-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Lists API
  slug: sharepoint-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-lists-api-openapi.yml
- filename: sharepoint-search-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Search API
  slug: sharepoint-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-search-api-openapi.yml
- filename: sharepoint-sites-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Sites API
  slug: sharepoint-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-sites-api-openapi.yml
- filename: sharepoint-user-profiles-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint User Profiles API
  slug: sharepoint-user-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-user-profiles-api-openapi.yml
- filename: sharepoint-batch-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint $batch API
  slug: microsoft-sharepoint-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-batch-api-openapi.yml
- filename: sharepoint-listitems-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint ListItems API
  slug: microsoft-sharepoint-listitems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-listitems-api-openapi.yml
- filename: sharepoint-site-api-openapi.yml
  format: yaml
  label: Microsoft SharePoint Site API
  slug: microsoft-sharepoint-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sharepoint/openapi/sharepoint-site-api-openapi.yml
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
name: Sharepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft SharePoint, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft SharePoint
provider_slug: sharepoint
slug: sharepoint-domain-security
source_filename: sharepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sharepoint/security/sharepoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
---
