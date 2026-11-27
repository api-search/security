---
api_specs:
- filename: openapi.json
  format: json
  label: Hera Fertility API
  slug: hera-fertility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/herafertility-co/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: herafertility.co
  spf: true
hosts:
- cert_expires: Jan 30 00:29:20 2027 GMT
  host: herafertility.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hera Fertility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hera Fertility, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hera Fertility
provider_slug: herafertility-co
slug: herafertility-co-domain-security
source_filename: herafertility-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: herafertility.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 00:29:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: herafertility.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/herafertility-co/security/herafertility-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fertility
- Healthcare
- Marketplace
- MaleHealth
---
