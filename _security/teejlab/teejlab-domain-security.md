---
api_specs:
- filename: teejlab-openapi-generated.yml
  format: yaml
  label: TeejLab API
  slug: teejlab-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teejlab/openapi/_ae-authored/teejlab-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: teejlab.com
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: teejlab.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Teejlab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeejLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TeejLab
provider_slug: teejlab
slug: teejlab-domain-security
source_filename: teejlab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teejlab.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: teejlab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/teejlab/security/teejlab-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- API Discovery
- API Security
- API Governance
- API Marketplace
- API Monetization
- DevSecOps
- Compliance
---
