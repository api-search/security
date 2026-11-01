---
api_specs:
- filename: amptoken-org-openapi-generated.yml
  format: yaml
  label: Amp API
  slug: amptoken-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amptoken-org/openapi/_ae-authored/amptoken-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amptoken.org
  spf: true
hosts:
- cert_expires: Jan 16 07:37:03 2027 GMT
  host: amptoken.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amptoken Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Amp
provider_slug: amptoken-org
slug: amptoken-org-domain-security
source_filename: amptoken-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amptoken.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 07:37:03 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amptoken.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/amptoken-org/security/amptoken-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Finance
- Blockchain
- Token
- Payments
---
