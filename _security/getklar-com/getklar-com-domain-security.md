---
api_specs:
- filename: getklar-com-openapi-generated.yml
  format: yaml
  label: Klar API
  slug: getklar-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getklar-com/openapi/_ae-authored/getklar-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getklar.com
  spf: true
hosts:
- cert_expires: Jan 21 10:08:57 2027 GMT
  host: getklar.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Klar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Klar
provider_slug: getklar-com
slug: getklar-com-domain-security
source_filename: getklar-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getklar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 10:08:57 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: getklar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getklar-com/security/getklar-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Marketing
- Analytics
- Attribution
- Software-as-a-Service
---
