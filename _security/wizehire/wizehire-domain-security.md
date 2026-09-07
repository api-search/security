---
api_specs:
- filename: wizehire-scout-service-openapi.yml
  format: yaml
  label: Wizehire Scout Service API
  slug: wizehire-scout-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wizehire/refs/heads/main/openapi/wizehire-scout-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wizehire.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: wizehire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: scout.wizehire.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Wizehire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WizeHire, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WizeHire
provider_slug: wizehire
slug: wizehire-domain-security
source_filename: wizehire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wizehire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: scout.wizehire.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wizehire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wizehire/refs/heads/main/security/wizehire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hiring
- Recruiting
- Applicant Tracking
- Human Resources
- Talent Assessment
- Small Business
- Artificial Intelligence
- Job Boards
- Onboarding
- HR Tech
---
