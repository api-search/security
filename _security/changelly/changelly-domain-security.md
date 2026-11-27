---
api_specs:
- filename: changelly-openapi-generated.yml
  format: yaml
  label: Changelly API
  slug: changelly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changelly/openapi/_ae-authored/changelly-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: changelly.com
  spf: true
hosts:
- cert_expires: Feb  2 06:59:06 2027 GMT
  host: changelly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Changelly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Changelly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Changelly
provider_slug: changelly
slug: changelly-domain-security
source_filename: changelly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: changelly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 06:59:06 2027 GMT\n  hsts: false\ndomains:\n- domain: changelly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/changelly/security/changelly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Fintech
---
