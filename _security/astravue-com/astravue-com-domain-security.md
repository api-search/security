---
api_specs:
- filename: astravue-com-openapi-generated.yml
  format: yaml
  label: Astravue API
  slug: astravue-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astravue-com/openapi/_ae-authored/astravue-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astravue.com
  spf: true
hosts:
- cert_expires: Jan 20 02:56:41 2027 GMT
  host: astravue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Astravue Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astravue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Astravue
provider_slug: astravue-com
slug: astravue-com-domain-security
source_filename: astravue-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astravue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 02:56:41 2027 GMT\n  hsts: false\ndomains:\n- domain: astravue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/astravue-com/security/astravue-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Project Management
- Profitability
- Software-as-a-Service
- Agencies
- Professional Services
---
