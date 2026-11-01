---
api_specs:
- filename: commenda-openapi-generated.yml
  format: yaml
  label: Commenda API
  slug: commenda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commenda/openapi/_ae-authored/commenda-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commenda.io
  spf: true
hosts:
- cert_expires: Nov 21 21:38:36 2026 GMT
  host: commenda.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Commenda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commenda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Commenda
provider_slug: commenda
slug: commenda-domain-security
source_filename: commenda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commenda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 21:38:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: commenda.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/commenda/security/commenda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Compliance
- Global
- Tax
---
