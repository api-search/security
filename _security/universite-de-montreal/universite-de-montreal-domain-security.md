---
api_specs:
- filename: universite-de-montreal-borealis-dataverse.yaml
  format: yaml
  label: UdeM Borealis Dataverse
  slug: borealis-dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universite-de-montreal/refs/heads/main/openapi/universite-de-montreal-borealis-dataverse.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: umontreal.ca
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.umontreal.ca
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: wiki.umontreal.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: papyrus.bib.umontreal.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Universite De Montreal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Université de Montréal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Université de Montréal
provider_slug: universite-de-montreal
slug: universite-de-montreal-domain-security
source_filename: universite-de-montreal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.umontreal.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n- host: wiki.umontreal.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: papyrus.bib.umontreal.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: umontreal.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universite-de-montreal/refs/heads/main/security/universite-de-montreal-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- Canada
- Québec
---
