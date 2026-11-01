---
api_specs:
- filename: curagent-io-openapi-generated.yml
  format: yaml
  label: curagent-io API
  slug: curagent-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/curagent-io/openapi/_ae-authored/curagent-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: curagent.io
  spf: true
hosts:
- cert_expires: Apr 27 23:59:59 2027 GMT
  host: curagent.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curagent Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for curagent-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: curagent-io
provider_slug: curagent-io
slug: curagent-io-domain-security
source_filename: curagent-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curagent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: curagent.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/curagent-io/security/curagent-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Title
- Risk Analysis
- API
- Document Processing
- Company
---
