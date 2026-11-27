---
api_specs:
- filename: nomado24-de-public-api-openapi.yml
  format: yaml
  label: Nomado24 Public API
  slug: nomado24-de-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nomado24-de/openapi/nomado24-de-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nomado24.de
  spf: true
hosts:
- cert_expires: Apr 29 23:59:59 2027 GMT
  host: nomado24.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nomado24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomado24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nomado24
provider_slug: nomado24-de
slug: nomado24-de-domain-security
source_filename: nomado24-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomado24.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nomado24.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nomado24-de/security/nomado24-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Remote Jobs
- Artificial Intelligence
- Germany
- Europe
- Job Search
---
