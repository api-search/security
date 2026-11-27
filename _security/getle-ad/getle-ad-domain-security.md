---
api_specs:
- filename: getle-ad-openapi-generated.yml
  format: yaml
  label: Getlead API
  slug: getle-ad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getle-ad/openapi/_ae-authored/getle-ad-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getle.ad
  spf: true
hosts:
- cert_expires: Jan 31 10:31:22 2027 GMT
  host: getle.ad
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getlead Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getlead, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Getlead
provider_slug: getle-ad
slug: getle-ad-domain-security
source_filename: getle-ad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getle.ad\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 10:31:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getle.ad\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getle-ad/security/getle-ad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Lead Generation
- Email Automation
- B2B Sales
- Artificial Intelligence
---
