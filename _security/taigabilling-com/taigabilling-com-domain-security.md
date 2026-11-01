---
api_specs:
- filename: taigabilling-com-openapi-generated.yml
  format: yaml
  label: Taiga API
  slug: taigabilling-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/taigabilling-com/openapi/_ae-authored/taigabilling-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: taigabilling.com
  spf: false
hosts:
- cert_expires: Jan 22 05:47:12 2027 GMT
  host: taigabilling.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taigabilling Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taiga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Taiga
provider_slug: taigabilling-com
slug: taigabilling-com-domain-security
source_filename: taigabilling-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taigabilling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 05:47:12 2027 GMT\n  hsts: false\ndomains:\n- domain: taigabilling.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/taigabilling-com/security/taigabilling-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- MedicalBilling
- Healthcare
- SaaS
- Automation
---
