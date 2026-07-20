---
api_specs:
- filename: civicplus-seeclickfix-open311-openapi-original.yml
  format: yaml
  label: SeeClickFix API v2
  slug: seeclickfix-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/civicplus/refs/heads/main/openapi/civicplus-seeclickfix-open311-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: civicplus.com
  spf: true
hosts:
- cert_expires: Oct  4 16:47:13 2026 GMT
  host: www.civicplus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Civicplus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CivicPlus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CivicPlus
provider_slug: civicplus
slug: civicplus-domain-security
source_filename: civicplus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.civicplus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:47:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: civicplus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civicplus/refs/heads/main/security/civicplus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- GovTech
- Local Government
- 311
- Civic Engagement
- Public Records
- Service Requests
---
