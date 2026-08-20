---
api_specs:
- filename: microsoft-onenote-notebooks-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Notebooks API
  slug: microsoft-onenote-notebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/openapi/microsoft-onenote-notebooks-api-openapi.yml
- filename: microsoft-onenote-pages-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Pages API
  slug: microsoft-onenote-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/openapi/microsoft-onenote-pages-api-openapi.yml
- filename: microsoft-onenote-sectiongroups-api-openapi.yml
  format: yaml
  label: Microsoft OneNote SectionGroups API
  slug: microsoft-onenote-sectiongroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/openapi/microsoft-onenote-sectiongroups-api-openapi.yml
- filename: microsoft-onenote-sections-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Sections API
  slug: microsoft-onenote-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/openapi/microsoft-onenote-sections-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
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
- cert_expires: Jan  5 19:53:18 2027 GMT
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
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Onenote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft OneNote, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microsoft OneNote
provider_slug: microsoft-onenote
slug: microsoft-onenote-domain-security
source_filename: microsoft-onenote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-onenote/refs/heads/main/security/microsoft-onenote-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Microsoft
- Microsoft-365
- Notebooks
- Notes
- Productivity
---
