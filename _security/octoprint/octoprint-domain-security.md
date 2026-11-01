---
api_specs:
- filename: octoprint-openapi-generated.yml
  format: yaml
  label: OctoPrint API
  slug: octoprint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octoprint/openapi/_ae-authored/octoprint-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: octoprint.org
  spf: true
hosts:
- cert_expires: Dec 24 18:48:44 2026 GMT
  host: octoprint.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Octoprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OctoPrint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OctoPrint
provider_slug: octoprint
slug: octoprint-domain-security
source_filename: octoprint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octoprint.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 18:48:44 2026 GMT\n  hsts: false\ndomains:\n- domain: octoprint.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/octoprint/security/octoprint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- 3D Printing
- Open Source
- IoT
- Maker
---
