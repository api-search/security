---
api_specs:
- filename: usedefinite-com-openapi-generated.yml
  format: yaml
  label: Definite API
  slug: usedefinite-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usedefinite-com/openapi/_ae-authored/usedefinite-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usedefinite.com
  spf: true
hosts:
- cert_expires: Dec 10 14:46:22 2026 GMT
  host: www.usedefinite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usedefinite Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Definite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Definite
provider_slug: usedefinite-com
slug: usedefinite-com-domain-security
source_filename: usedefinite-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usedefinite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 14:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usedefinite.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/usedefinite-com/security/usedefinite-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Ontology
- Integration
- SaaS
---
