---
api_specs:
- filename: prophaze-openapi-generated.yml
  format: yaml
  label: prophaze API
  slug: prophaze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prophaze/openapi/_ae-authored/prophaze-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: prophaze.com
  spf: true
hosts:
- host: prophaze.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prophaze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for prophaze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: prophaze
provider_slug: prophaze
slug: prophaze-domain-security
source_filename: prophaze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prophaze.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: prophaze.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/prophaze/security/prophaze-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Security
- AI
- WAAP
- Enterprise
---
