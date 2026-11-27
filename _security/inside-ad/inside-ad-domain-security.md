---
api_specs:
- filename: inside-ad-openapi-generated.yml
  format: yaml
  label: Inside API
  slug: inside-ad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inside-ad/openapi/_ae-authored/inside-ad-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: inside.ad
  spf: true
hosts:
- cert_expires: Jan 29 11:57:31 2027 GMT
  host: inside.ad
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inside Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inside, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Inside
provider_slug: inside-ad
slug: inside-ad-domain-security
source_filename: inside-ad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inside.ad\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 11:57:31 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inside.ad\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inside-ad/security/inside-ad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Creator Platform
- Advertising
- Monetization
- Collaboration
- Platform
---
