---
api_specs:
- filename: secondfactor-openapi-generated.yml
  format: yaml
  label: SecondFactor API
  slug: secondfactor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/secondfactor/openapi/_ae-authored/secondfactor-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: secondfactor.ai
  spf: true
hosts:
- cert_expires: Dec 16 15:45:02 2026 GMT
  host: secondfactor.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 08:14:28 2027 GMT
  host: docs.secondfactor.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: api.secondfactor.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: SecondFactor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SecondFactor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SecondFactor
provider_slug: secondfactor
slug: secondfactor-domain-security
source_filename: secondfactor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secondfactor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:45:02 2026 GMT\n  hsts: false\n- host: docs.secondfactor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 08:14:28 2027 GMT\n  hsts: false\n- host: api.secondfactor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: secondfactor.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/secondfactor/security/secondfactor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- OTP
- Authentication
- Multi-Channel
- Messaging
---
