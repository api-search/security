---
api_specs:
- filename: axiomatics-authorize-api-openapi.yml
  format: yaml
  label: Axiomatics Authorize API
  slug: axiomatics-authorize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomatics/openapi/axiomatics-authorize-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axiomatics.com
  spf: true
hosts:
- cert_expires: Dec 15 11:36:14 2026 GMT
  host: axiomatics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axiomatics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axiomatics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axiomatics
provider_slug: axiomatics
slug: axiomatics-domain-security
source_filename: axiomatics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axiomatics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 11:36:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axiomatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/axiomatics/security/axiomatics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Authorization
- Policy
- ZeroTrust
- Compliance
- Enterprise
---
