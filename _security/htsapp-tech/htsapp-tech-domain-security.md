---
api_specs:
- filename: htsapp-tech-meta-api-openapi.yml
  format: yaml
  label: HTSApp Meta API
  slug: htsapp-tech-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/htsapp-tech/openapi/htsapp-tech-meta-api-openapi.yml
- filename: htsapp-tech-paid-api-openapi.yml
  format: yaml
  label: HTSApp Paid API
  slug: htsapp-tech-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/htsapp-tech/openapi/htsapp-tech-paid-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: htsapp.tech
  spf: false
hosts:
- cert_expires: Jan 25 15:46:43 2027 GMT
  host: htsapp.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HTSApp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HTSApp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HTSApp
provider_slug: htsapp-tech
slug: htsapp-tech-domain-security
source_filename: htsapp-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: htsapp.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 15:46:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: htsapp.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/htsapp-tech/security/htsapp-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Mobile
- Application
- Privacy
- Gaming
---
