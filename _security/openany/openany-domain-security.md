---
api_specs:
- filename: openany-openapi-generated.yml
  format: yaml
  label: OpenAny API
  slug: openany-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openany/openapi/_ae-authored/openany-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openany.si
  spf: true
hosts:
- cert_expires: Jan 14 08:07:25 2027 GMT
  host: openany.si
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openany Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAny, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenAny
provider_slug: openany
slug: openany-domain-security
source_filename: openany-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openany.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 08:07:25 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: openany.si\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openany/security/openany-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Marketplace
- Agents
- Models
---
