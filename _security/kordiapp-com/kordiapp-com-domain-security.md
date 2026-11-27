---
api_specs:
- filename: kordiapp-com-openapi-generated.yml
  format: yaml
  label: Kordi API
  slug: kordiapp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kordiapp-com/openapi/_ae-authored/kordiapp-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kordiapp.com
  spf: true
hosts:
- cert_expires: Feb 11 05:33:45 2027 GMT
  host: kordiapp.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kordi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kordi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kordi
provider_slug: kordiapp-com
slug: kordiapp-com-domain-security
source_filename: kordiapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kordiapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 05:33:45 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: kordiapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kordiapp-com/security/kordiapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Streaming Services
- Trial Tracking
- API Platform
- Entertainment Recommendations
---
