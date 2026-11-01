---
api_specs:
- filename: mojeek-search-api-openapi.yml
  format: yaml
  label: Mojeek Search API
  slug: mojeek-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mojeek/openapi/mojeek-search-api-openapi.yml
- filename: mojeek-openapi-generated.yml
  format: yaml
  label: Mojeek API
  slug: mojeek-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mojeek/openapi/_ae-authored/mojeek-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mojeek.com
  spf: true
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: www.mojeek.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mojeek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mojeek, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mojeek
provider_slug: mojeek
slug: mojeek-domain-security
source_filename: mojeek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mojeek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mojeek.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mojeek/security/mojeek-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Search
- Privacy
- API
- Open-source
- Community
---
