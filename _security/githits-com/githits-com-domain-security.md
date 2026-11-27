---
api_specs:
- filename: githits-com-openapi-generated.yml
  format: yaml
  label: GitHits API
  slug: githits-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/githits-com/openapi/_ae-authored/githits-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: githits.com
  spf: true
hosts:
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: githits.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GitHits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitHits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GitHits
provider_slug: githits-com
slug: githits-com-domain-security
source_filename: githits-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: githits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: githits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/githits-com/security/githits-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Source
- Artificial Intelligence
- Coding Agents
- Indexing
- Platform
---
