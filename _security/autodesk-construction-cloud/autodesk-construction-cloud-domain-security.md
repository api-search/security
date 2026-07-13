---
api_specs:
- filename: acc-admin-openapi.yml
  format: yaml
  label: Autodesk Construction Cloud Admin API
  slug: acc-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/openapi/acc-admin-openapi.yml
- filename: acc-issues-openapi.yml
  format: yaml
  label: Autodesk Construction Cloud Issues API
  slug: acc-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/openapi/acc-issues-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: autodesk.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.autodesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: aps.autodesk.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: developer.api.autodesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autodesk Construction Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autodesk Construction Cloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Autodesk Construction Cloud
provider_slug: autodesk-construction-cloud
slug: autodesk-construction-cloud-domain-security
source_filename: autodesk-construction-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\n- host: aps.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.api.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: autodesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/security/autodesk-construction-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Construction
- BIM
- Project Management
- AEC
- CAD
- Architecture
- Engineering
- Field Management
---
