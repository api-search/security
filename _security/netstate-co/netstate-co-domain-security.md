---
api_specs:
- filename: netstate-co-openapi-generated.yml
  format: yaml
  label: Netstate API
  slug: netstate-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netstate-co/openapi/_ae-authored/netstate-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netstate.co
  spf: false
hosts:
- cert_expires: Feb  7 03:30:45 2027 GMT
  host: netstate.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netstate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netstate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Netstate
provider_slug: netstate-co
slug: netstate-co-domain-security
source_filename: netstate-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netstate.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 03:30:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netstate.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/netstate-co/security/netstate-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business
- Data
- KYB
- Verification
---
