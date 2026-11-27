---
api_specs:
- filename: mana-am-agents-api-openapi.yml
  format: yaml
  label: Mana Agents API
  slug: mana-am-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mana-am/openapi/mana-am-agents-api-openapi.yml
- filename: mana-am-apps-api-openapi.yml
  format: yaml
  label: Mana Apps API
  slug: mana-am-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mana-am/openapi/mana-am-apps-api-openapi.yml
- filename: mana-am-community-api-openapi.yml
  format: yaml
  label: Mana Community API
  slug: mana-am-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mana-am/openapi/mana-am-community-api-openapi.yml
- filename: mana-am-discovery-api-openapi.yml
  format: yaml
  label: Mana Discovery API
  slug: mana-am-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mana-am/openapi/mana-am-discovery-api-openapi.yml
- filename: mana-am-users-api-openapi.yml
  format: yaml
  label: Mana Users API
  slug: mana-am-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mana-am/openapi/mana-am-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mana.am
  spf: true
hosts:
- cert_expires: Jan 29 08:25:59 2027 GMT
  host: mana.am
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mana
provider_slug: mana-am
slug: mana-am-domain-security
source_filename: mana-am-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mana.am\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 08:25:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mana.am\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mana-am/security/mana-am-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Personal Agent
- iPhone
- No-Code
- Creative Tools
---
