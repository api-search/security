---
api_specs:
- filename: dvt-dev-openapi-generated.yml
  format: yaml
  label: flurry API
  slug: dvt-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dvt-dev/openapi/_ae-authored/dvt-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dvt.dev
  spf: true
hosts:
- cert_expires: Jan  1 08:09:56 2027 GMT
  host: dvt.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dvt Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flurry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: flurry
provider_slug: dvt-dev
slug: dvt-dev-domain-security
source_filename: dvt-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dvt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 08:09:56 2027 GMT\n  hsts: false\ndomains:\n- domain: dvt.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dvt-dev/security/dvt-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Data Apps
- Snowflake
- Platform
---
