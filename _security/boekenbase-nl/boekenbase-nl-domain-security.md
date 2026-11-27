---
api_specs:
- filename: boekenbase-nl-v1-openapi.json
  format: json
  label: Boekenbase API V1 API
  slug: boekenbase-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boekenbase-nl/openapi/_original/boekenbase-nl-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: boekenbase.nl
  spf: false
hosts:
- cert_expires: Dec 27 03:32:40 2026 GMT
  host: boekenbase.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BoekenBase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoekenBase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: BoekenBase
provider_slug: boekenbase-nl
slug: boekenbase-nl-domain-security
source_filename: boekenbase-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boekenbase.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 03:32:40 2026 GMT\n  hsts: false\ndomains:\n- domain: boekenbase.nl\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/boekenbase-nl/security/boekenbase-nl-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Books
- Catalog
- Netherlands
- Library
---
