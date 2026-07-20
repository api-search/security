---
api_specs:
- filename: sharepoint-rest-openapi.json
  format: json
  label: SharePoint REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://example.com/sharepoint-rest-openapi.json
- filename: graph-sharepoint-openapi.json
  format: json
  label: Microsoft Graph API (SharePoint)
  slug: graph-api-sharepoint
  spec_type: OpenAPI
  url: https://example.com/graph-sharepoint-openapi.json
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
  spf_record: v=spf1 include:_spf-a.microsoft.com include:_spf-b.microsoft.com include:_spf-c.microsoft.com include:_spf-ssg-a.msft.net include:_spf1-meo.microsoft.com -all
hosts:
- host: graph.microsoft.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: login.microsoftonline.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sharepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft SharePoint, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft SharePoint
provider_slug: sharepoint
slug: sharepoint-domain-security
source_filename: sharepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: probed\nnotes: >-\n  SharePoint REST baseURLs are tenant-templated (https://{site_url}/_api) with no fixed host,\n  so the automated probe reported no-hosts. The hosts below were probed directly: the identity\n  host (login.microsoftonline.com), the Microsoft Graph host (graph.microsoft.com), and the\n  corporate web host (www.microsoft.com). Domain-level DNS records are for microsoft.com.\nhosts:\n  - {host: graph.microsoft.com, https: true, tls_version: TLSv1.3, hsts: true, hsts_max_age: 31536000, hsts_include_subdomains: false}\n  - {host: login.microsoftonline.com, https: true, tls_version: TLSv1.3, hsts: true, hsts_max_age: 31536000, hsts_include_subdomains: true}\n  - {host: www.microsoft.com, https: true, tls_version: TLSv1.3, hsts: false}\ndomains:\n  - domain: microsoft.com\n    dnssec: false\n    caa: ['0 contactemail \"caarecordaware@microsoft.com\"']\n    spf: true\n    spf_record: \"v=spf1 include:_spf-a.microsoft.com include:_spf-b.microsoft.com\
  \ include:_spf-c.microsoft.com include:_spf-ssg-a.msft.net include:_spf1-meo.microsoft.com -all\"\n    dmarc: true\n    dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/security/sharepoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
---
