---
api_specs:
- filename: defade-org-openapi-generated.yml
  format: yaml
  label: DeFade API
  slug: defade-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/defade-org/openapi/_ae-authored/defade-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: defade.org
  spf: true
hosts:
- cert_expires: Jan  9 13:06:01 2027 GMT
  host: defade.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Defade Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeFade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DeFade
provider_slug: defade-org
slug: defade-org-domain-security
source_filename: defade-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: defade.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 13:06:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: defade.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/defade-org/security/defade-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Security
- Analytics
- Multi-Chain
- DeFi
---
