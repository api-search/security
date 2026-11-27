---
api_specs:
- filename: homecalc-ca-openapi-generated.yml
  format: yaml
  label: HomeCalc.ca API
  slug: homecalc-ca-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/homecalc-ca/openapi/_ae-authored/homecalc-ca-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: homecalc.ca
  spf: true
hosts:
- cert_expires: Dec 19 20:21:09 2026 GMT
  host: homecalc.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HomeCalc.ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HomeCalc.ca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HomeCalc.ca
provider_slug: homecalc-ca
slug: homecalc-ca-domain-security
source_filename: homecalc-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homecalc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 20:21:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: homecalc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/homecalc-ca/security/homecalc-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Mortgage
- Calculators
- Canada
---
