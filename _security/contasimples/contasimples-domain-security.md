---
api_specs:
- filename: contasimples-openapi-generated.yml
  format: yaml
  label: Contasimples API
  slug: contasimples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/openapi/_ae-authored/contasimples-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: contasimples.com
  spf: true
hosts:
- cert_expires: Dec 12 17:58:43 2026 GMT
  host: contasimples.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contasimples Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contasimples, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Contasimples
provider_slug: contasimples
slug: contasimples-domain-security
source_filename: contasimples-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contasimples.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 17:58:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: contasimples.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contasimples/refs/heads/main/security/contasimples-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
