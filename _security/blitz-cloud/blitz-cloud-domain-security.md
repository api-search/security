---
api_specs:
- filename: blitz-cloud-openapi-generated.yml
  format: yaml
  label: BlitzWorks API
  slug: blitz-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blitz-cloud/openapi/_ae-authored/blitz-cloud-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: blitz.cloud
  spf: true
hosts:
- cert_expires: Jan 31 19:04:08 2027 GMT
  host: blitz.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BlitzWorks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlitzWorks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BlitzWorks
provider_slug: blitz-cloud
slug: blitz-cloud-domain-security
source_filename: blitz-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blitz.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 19:04:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blitz.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blitz-cloud/security/blitz-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Hosting
- EU
- Application
- Bots
- Artificial Intelligence
- Company
---
