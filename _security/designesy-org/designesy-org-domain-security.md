---
api_specs:
- filename: designesy-org-openapi-generated.yml
  format: yaml
  label: designesy-org API
  slug: designesy-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/designesy-org/openapi/_ae-authored/designesy-org-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: designesy.org
  spf: true
hosts:
- cert_expires: Dec 10 15:52:22 2026 GMT
  host: designesy.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Designesy Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for designesy-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: designesy-org
provider_slug: designesy-org
slug: designesy-org-domain-security
source_filename: designesy-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: designesy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 15:52:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: designesy.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/designesy-org/security/designesy-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Design verification
- Design contracts
- UI scoring
- Accessibility checks
- Motion Graphics
- Design Tokens
- Developer Tools
---
