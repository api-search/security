---
api_specs:
- filename: leadrecorder-com-openapi-generated.yml
  format: yaml
  label: Lead Recorder API
  slug: leadrecorder-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadrecorder-com/openapi/_ae-authored/leadrecorder-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leadrecorder.com
  spf: true
hosts:
- cert_expires: Feb  1 04:07:24 2027 GMT
  host: leadrecorder.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lead Recorder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lead Recorder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lead Recorder
provider_slug: leadrecorder-com
slug: leadrecorder-com-domain-security
source_filename: leadrecorder-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadrecorder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 04:07:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: leadrecorder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leadrecorder-com/security/leadrecorder-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Attribution
- Lead Tracking
- Software-as-a-Service
- Analytics
---
