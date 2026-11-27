---
api_specs:
- filename: heista-co-account-api-openapi.yml
  format: yaml
  label: Heista Account API
  slug: heista-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heista-co/openapi/heista-co-account-api-openapi.yml
- filename: heista-co-adscript-api-openapi.yml
  format: yaml
  label: Heista Adscript API
  slug: heista-co-adscript-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heista-co/openapi/heista-co-adscript-api-openapi.yml
- filename: heista-co-decode-api-openapi.yml
  format: yaml
  label: Heista Decode API
  slug: heista-co-decode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heista-co/openapi/heista-co-decode-api-openapi.yml
- filename: heista-co-files-api-openapi.yml
  format: yaml
  label: Heista Files API
  slug: heista-co-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heista-co/openapi/heista-co-files-api-openapi.yml
- filename: heista-co-intelligence-api-openapi.yml
  format: yaml
  label: Heista Intelligence API
  slug: heista-co-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heista-co/openapi/heista-co-intelligence-api-openapi.yml
- filename: heista-co-powersource-api-openapi.yml
  format: yaml
  label: Heista Power Source API
  slug: heista-co-powersource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heista-co/openapi/heista-co-powersource-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heista.co
  spf: true
hosts:
- cert_expires: Jan  5 19:24:02 2027 GMT
  host: heista.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heista Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heista, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Heista
provider_slug: heista-co
slug: heista-co-domain-security
source_filename: heista-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heista.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:24:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: heista.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/heista-co/security/heista-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Creative
- Agency
- Workspace
- Platform
---
