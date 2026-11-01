---
api_specs:
- filename: klever-org-openapi-generated.yml
  format: yaml
  label: klever-org API
  slug: klever-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klever-org/openapi/_ae-authored/klever-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: klever.org
  spf: true
hosts:
- cert_expires: Jan 14 01:28:08 2027 GMT
  host: klever.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Klever Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for klever-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: klever-org
provider_slug: klever-org
slug: klever-org-domain-security
source_filename: klever-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klever.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 01:28:08 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: klever.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/klever-org/security/klever-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Crypto
- Smart-Contracts
- Developer-Platform
---
