---
api_specs:
- filename: musael-com-public-api-openapi.yml
  format: yaml
  label: Musael Public API
  slug: musael-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musael-com/openapi/musael-com-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: musael.com
  spf: true
hosts:
- cert_expires: Dec 26 19:46:55 2026 GMT
  host: musael.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Musael Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Musael, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Musael
provider_slug: musael-com
slug: musael-com-domain-security
source_filename: musael-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: musael.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 19:46:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: musael.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/musael-com/security/musael-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Author Tools
- Name Generators
---
