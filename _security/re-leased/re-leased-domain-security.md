---
api_specs:
- filename: re-leased-openapi-generated.yml
  format: yaml
  label: Re-Leased API
  slug: re-leased-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/re-leased/openapi/_ae-authored/re-leased-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: re-leased.com
  spf: true
hosts:
- cert_expires: Jan 25 01:41:04 2027 GMT
  host: www.re-leased.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Re-Leased Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Re-Leased, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Re-Leased
provider_slug: re-leased
slug: re-leased-domain-security
source_filename: re-leased-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.re-leased.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 01:41:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: re-leased.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/re-leased/security/re-leased-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Management
- Software-as-a-Service
- Commercial Software
- Re-Leased
---
