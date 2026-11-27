---
api_specs:
- filename: buildwithgage-com-openapi-generated.yml
  format: yaml
  label: Gage API
  slug: buildwithgage-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildwithgage-com/openapi/_ae-authored/buildwithgage-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buildwithgage.com
  spf: true
hosts:
- cert_expires: Dec  8 16:45:35 2026 GMT
  host: buildwithgage.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gage
provider_slug: buildwithgage-com
slug: buildwithgage-com-domain-security
source_filename: buildwithgage-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildwithgage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 16:45:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buildwithgage.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buildwithgage-com/security/buildwithgage-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Marketplace
- Steel
- Developers
---
