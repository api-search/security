---
api_specs:
- filename: lightbringer-com-oauth-api-openapi.yml
  format: yaml
  label: Lightbringer OAuth API
  slug: lightbringer-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-oauth-api-openapi.yml
- filename: lightbringer-com-public-api-openapi.yml
  format: yaml
  label: Lightbringer Public API
  slug: lightbringer-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-public-api-openapi.yml
- filename: lightbringer-com-well-known-api-openapi.yml
  format: yaml
  label: Lightbringer .well Known API
  slug: lightbringer-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lightbringer-com/openapi/lightbringer-com-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightbringer.com
  spf: true
hosts:
- cert_expires: Jan 18 00:46:16 2027 GMT
  host: lightbringer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lightbringer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightbringer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lightbringer
provider_slug: lightbringer-com
slug: lightbringer-com-domain-security
source_filename: lightbringer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightbringer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 00:46:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightbringer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lightbringer-com/security/lightbringer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Patents
- Deep Tech
- Startups
- Platform
---
