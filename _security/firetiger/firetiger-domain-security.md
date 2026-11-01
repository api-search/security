---
api_specs:
- filename: firetiger-openapi-generated.yml
  format: yaml
  label: Firetiger API
  slug: firetiger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firetiger/openapi/_ae-authored/firetiger-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firetiger.com
  spf: true
hosts:
- cert_expires: Dec 27 21:02:16 2026 GMT
  host: firetiger.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firetiger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firetiger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Firetiger
provider_slug: firetiger
slug: firetiger-domain-security
source_filename: firetiger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firetiger.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 21:02:16 2026 GMT\n  hsts: null\ndomains:\n- domain: firetiger.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/firetiger/security/firetiger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Startup
- Venture-Backed
- Technology
- API
---
