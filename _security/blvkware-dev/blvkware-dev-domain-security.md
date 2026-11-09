---
api_specs:
- filename: blvkware-dev-check-api-openapi.yml
  format: yaml
  label: BlvkWare Check API
  slug: blvkware-dev-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvkware-dev/openapi/blvkware-dev-check-api-openapi.yml
- filename: blvkware-dev-corpus-api-openapi.yml
  format: yaml
  label: BlvkWare Corpus API
  slug: blvkware-dev-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvkware-dev/openapi/blvkware-dev-corpus-api-openapi.yml
- filename: blvkware-dev-meta-api-openapi.yml
  format: yaml
  label: BlvkWare Meta API
  slug: blvkware-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvkware-dev/openapi/blvkware-dev-meta-api-openapi.yml
- filename: blvkware-dev-watch-api-openapi.yml
  format: yaml
  label: BlvkWare Watch API
  slug: blvkware-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blvkware-dev/openapi/blvkware-dev-watch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: blvkware.dev
  spf: true
hosts:
- cert_expires: Jan  5 17:32:21 2027 GMT
  host: blvkware.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blvkware Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlvkWare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BlvkWare
provider_slug: blvkware-dev
slug: blvkware-dev-domain-security
source_filename: blvkware-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blvkware.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 17:32:21 2027 GMT\n  hsts: false\ndomains:\n- domain: blvkware.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blvkware-dev/security/blvkware-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Agents
- Kit
- Automation
- Marketplace
- Company
---
