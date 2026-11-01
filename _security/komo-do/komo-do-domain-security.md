---
api_specs:
- filename: komo-do-openapi-generated.yml
  format: yaml
  label: Komodo API
  slug: komo-do-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/komo-do/openapi/_ae-authored/komo-do-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: komo.do
  spf: false
hosts:
- cert_expires: Jan 21 00:33:22 2027 GMT
  host: komo.do
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Komo Do Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Komodo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Komodo
provider_slug: komo-do
slug: komo-do-domain-security
source_filename: komo-do-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: komo.do\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 00:33:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: komo.do\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/komo-do/security/komo-do-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- DevOps
- Infrastructure
- Automation
- OpenSource
---
