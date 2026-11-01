---
api_specs:
- filename: niva-openapi-generated.yml
  format: yaml
  label: Niva API
  slug: niva-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/niva/openapi/_ae-authored/niva-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: niva.co
  spf: true
hosts:
- cert_expires: Jan  8 18:45:12 2027 GMT
  host: www.niva.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Niva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Niva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Niva
provider_slug: niva
slug: niva-domain-security
source_filename: niva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.niva.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 18:45:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: niva.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/niva/security/niva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FinTech
- IdentityVerification
- AI
- Compliance
---
