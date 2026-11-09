---
api_specs:
- filename: flyweel-co-openapi-generated.yml
  format: yaml
  label: Flyweel API
  slug: flyweel-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyweel-co/openapi/_ae-authored/flyweel-co-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flyweel.co
  spf: true
hosts:
- cert_expires: Feb  2 06:15:43 2027 GMT
  host: flyweel.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flyweel Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flyweel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flyweel
provider_slug: flyweel-co
slug: flyweel-co-domain-security
source_filename: flyweel-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flyweel.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 06:15:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flyweel.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flyweel-co/security/flyweel-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising Finance
- Capital Cards
- Debit Cards
- Invoice Reconciliation
- Enterprise SaaS
---
