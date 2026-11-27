---
api_specs:
- filename: meridary-com-agent-api-openapi.yml
  format: yaml
  label: Meridary Agent API
  slug: meridary-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meridary-com/openapi/meridary-com-agent-api-openapi.yml
- filename: meridary-com-calculators-api-openapi.yml
  format: yaml
  label: Meridary Calculators API
  slug: meridary-com-calculators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meridary-com/openapi/meridary-com-calculators-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meridary.com
  spf: false
hosts:
- cert_expires: Jan  3 03:13:45 2027 GMT
  host: meridary.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meridary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meridary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Meridary
provider_slug: meridary-com
slug: meridary-com-domain-security
source_filename: meridary-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meridary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 03:13:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: meridary.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/meridary-com/security/meridary-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Retirement
- Planning
- Calculator
- Software-as-a-Service
---
