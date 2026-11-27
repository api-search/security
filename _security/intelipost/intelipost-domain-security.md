---
api_specs:
- filename: intelipost-openapi-generated.yml
  format: yaml
  label: Intelipost API
  slug: intelipost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intelipost/openapi/_ae-authored/intelipost-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intelipost.com.br
  spf: true
hosts:
- cert_expires: May 12 23:59:59 2027 GMT
  host: www.intelipost.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Intelipost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intelipost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Intelipost
provider_slug: intelipost
slug: intelipost-domain-security
source_filename: intelipost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intelipost.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: intelipost.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/intelipost/security/intelipost-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logistics
- Transportation
- Software-as-a-Service
- E-Commerce
---
