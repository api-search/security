---
api_specs:
- filename: planradar-openapi-original.json
  format: json
  label: PlanRadar Open API
  slug: planradar-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planradar/refs/heads/main/openapi/planradar-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: planradar.com
  spf: true
hosts:
- cert_expires: Sep 17 16:03:09 2026 GMT
  host: www.planradar.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planradar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlanRadar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PlanRadar
provider_slug: planradar
slug: planradar-domain-security
source_filename: planradar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.planradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:03:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: planradar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planradar/refs/heads/main/security/planradar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Construction
- Real Estate
- Project Management
- Documentation
- Defect Management
- Field Service
- Facility Management
- BIM
- SaaS
---
