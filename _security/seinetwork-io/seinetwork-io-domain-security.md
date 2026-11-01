---
api_specs:
- filename: seinetwork-io-openapi-generated.yml
  format: yaml
  label: Sei API
  slug: seinetwork-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/seinetwork-io/openapi/_ae-authored/seinetwork-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seinetwork.io
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: seinetwork.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seinetwork Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sei, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sei
provider_slug: seinetwork-io
slug: seinetwork-io-domain-security
source_filename: seinetwork-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seinetwork.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: seinetwork.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/seinetwork-io/security/seinetwork-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Infrastructure
- Finance
- DeFi
---
