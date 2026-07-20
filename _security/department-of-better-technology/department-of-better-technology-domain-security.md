---
api_specs:
- filename: department-of-better-technology-screendoor-openapi.yml
  format: yaml
  label: Screendoor API
  slug: screendoor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-screendoor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dobt.co
  spf: true
hosts:
- host: dobt.co
  https: false
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: screendoor.dobt.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Department Of Better Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Better Technology, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Department of Better Technology
provider_slug: department-of-better-technology
slug: department-of-better-technology-domain-security
source_filename: department-of-better-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dobt.co\n  https: false\n- host: screendoor.dobt.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dobt.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/security/department-of-better-technology-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Forms
- Government
- GovTech
- Civic Technology
- Workflow
- Data Collection
- Screendoor
- Public Sector
- Forms API
---
