---
api_specs:
- filename: finalcad-projects-openapi.yml
  format: yaml
  label: Finalcad One Project API
  slug: finalcad-one-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finalcad/refs/heads/main/openapi/finalcad-projects-openapi.yml
- filename: finalcad-organizations-openapi.yml
  format: yaml
  label: Finalcad One Organization Management API
  slug: finalcad-one-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finalcad/refs/heads/main/openapi/finalcad-organizations-openapi.yml
- filename: finalcad-medias-openapi.yml
  format: yaml
  label: Finalcad One Medias API
  slug: finalcad-one-medias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finalcad/refs/heads/main/openapi/finalcad-medias-openapi.yml
- filename: finalcad-webhooks-openapi.yml
  format: yaml
  label: Finalcad One Webhooks API
  slug: finalcad-one-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finalcad/refs/heads/main/openapi/finalcad-webhooks-openapi.yml
- filename: finalcad-libraries-openapi.yml
  format: yaml
  label: Finalcad One Libraries API
  slug: finalcad-one-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finalcad/refs/heads/main/openapi/finalcad-libraries-openapi.yml
- filename: finalcad-authentication-openapi.yml
  format: yaml
  label: Finalcad One Authentication API
  slug: finalcad-one-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finalcad/refs/heads/main/openapi/finalcad-authentication-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: finalcad.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: finalcad.cloud
  spf: false
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.finalcad.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: developer.finalcad.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: developer.sandbox.finalcad.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finalcad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finalcad, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Finalcad
provider_slug: finalcad
slug: finalcad-domain-security
source_filename: finalcad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finalcad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\n- host: developer.finalcad.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\n- host: developer.sandbox.finalcad.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: finalcad.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: finalcad.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finalcad/refs/heads/main/security/finalcad-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Construction
- Construction Technology
- Field Management
- Project Management
- Quality Control
- Safety
- BIM
- Documents
- Collaboration
- SaaS
---
