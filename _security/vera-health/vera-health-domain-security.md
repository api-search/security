---
api_specs:
- filename: vera-health-chat-api-openapi.yml
  format: yaml
  label: Vera Health Chat API
  slug: vera-health-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vera-health/openapi/vera-health-chat-api-openapi.yml
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
  domain: verahealth.ai
  spf: true
hosts:
- cert_expires: Dec 13 19:46:37 2026 GMT
  host: www.verahealth.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vera Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vera Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vera Health
provider_slug: vera-health
slug: vera-health-domain-security
source_filename: vera-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verahealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 19:46:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: verahealth.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/vera-health/security/vera-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- AI
- Clinical Decision Support
- Medical Knowledge
- Healthcare
---
