---
api_specs:
- filename: nameshift-com-openapi-generated.yml
  format: yaml
  label: Nameshift API
  slug: nameshift-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nameshift-com/openapi/_ae-authored/nameshift-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nameshift.com
  spf: true
hosts:
- cert_expires: Jan 13 02:11:34 2027 GMT
  host: nameshift.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nameshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nameshift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Nameshift
provider_slug: nameshift-com
slug: nameshift-com-domain-security
source_filename: nameshift-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nameshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 02:11:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: nameshift.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nameshift-com/security/nameshift-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketplace
- Domains
- Auctions
- E-Commerce
- Global
---
