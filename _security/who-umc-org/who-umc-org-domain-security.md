---
api_specs:
- filename: who-umc-org-openapi-generated.yml
  format: yaml
  label: Uppsala Monitoring Centre (WHO) API
  slug: who-umc-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/who-umc-org/openapi/_ae-authored/who-umc-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: who-umc.org
  spf: true
hosts:
- cert_expires: Jan 13 19:59:47 2027 GMT
  host: who-umc.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uppsala Monitoring Centre (WHO) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uppsala Monitoring Centre (WHO), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Uppsala Monitoring Centre (WHO)
provider_slug: who-umc-org
slug: who-umc-org-domain-security
source_filename: who-umc-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: who-umc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 19:59:47 2027 GMT\n  hsts: false\ndomains:\n- domain: who-umc.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/who-umc-org/security/who-umc-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmacovigilance
- Health
- Data Services
- WHO
---
