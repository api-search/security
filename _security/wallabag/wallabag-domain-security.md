---
api_specs:
- filename: wallabag-openapi-generated.yml
  format: yaml
  label: wallabag API
  slug: wallabag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wallabag/openapi/_ae-authored/wallabag-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wallabag.org
  spf: true
hosts:
- cert_expires: Jan 16 07:53:50 2027 GMT
  host: wallabag.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wallabag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wallabag, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: wallabag
provider_slug: wallabag
slug: wallabag-domain-security
source_filename: wallabag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wallabag.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 07:53:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wallabag.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/wallabag/security/wallabag-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Source
- Read-it-later
- Self-hosted
- Privacy
- Community
---
