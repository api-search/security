---
api_specs:
- filename: founderhood-app-openapi-generated.yml
  format: yaml
  label: Founderhood API
  slug: founderhood-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/founderhood-app/openapi/_ae-authored/founderhood-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: founderhood.app
  spf: true
hosts:
- cert_expires: Jan 23 07:15:26 2027 GMT
  host: founderhood.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Founderhood Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Founderhood, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Founderhood
provider_slug: founderhood-app
slug: founderhood-app-domain-security
source_filename: founderhood-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: founderhood.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 07:15:26 2027 GMT\n  hsts: false\ndomains:\n- domain: founderhood.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/founderhood-app/security/founderhood-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Community
- Directory
- Startups
- Entrepreneurs
- Indie Makers
---
