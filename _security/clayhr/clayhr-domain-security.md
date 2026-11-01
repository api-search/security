---
api_specs:
- filename: clayhr-openapi-generated.yml
  format: yaml
  label: ClayHR API
  slug: clayhr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clayhr/openapi/_ae-authored/clayhr-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clayhr.com
  spf: true
hosts:
- cert_expires: Jan 12 08:48:30 2027 GMT
  host: www.clayhr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clayhr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClayHR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ClayHR
provider_slug: clayhr
slug: clayhr-domain-security
source_filename: clayhr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clayhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 08:48:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clayhr.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/clayhr/security/clayhr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRMS
- SaaS
- AI
- Employee-Management
- Performance-Management
---
