---
api_specs:
- filename: directree-io-listings-api-openapi.yml
  format: yaml
  label: Directree Listings API
  slug: directree-io-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/directree-io/openapi/directree-io-listings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: directree.io
  spf: true
hosts:
- cert_expires: Feb  2 00:55:28 2027 GMT
  host: directree.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Directree Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Directree, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Directree
provider_slug: directree-io
slug: directree-io-domain-security
source_filename: directree-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: directree.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 00:55:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: directree.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/directree-io/security/directree-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software-as-a-Service
- Directory
- Software
- Reviews
- Open Data
---
