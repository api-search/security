---
api_specs:
- filename: pagelens-io-openapi-generated.yml
  format: yaml
  label: PageLens API
  slug: pagelens-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelens-io/openapi/_ae-authored/pagelens-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pagelens.io
  spf: true
hosts:
- cert_expires: Jan  5 05:23:54 2027 GMT
  host: pagelens.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PageLens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PageLens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PageLens
provider_slug: pagelens-io
slug: pagelens-io-domain-security
source_filename: pagelens-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagelens.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 05:23:54 2027 GMT\n  hsts: false\ndomains:\n- domain: pagelens.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pagelens-io/security/pagelens-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Artificial Intelligence
- Privacy
- Cookieless
- Web Analytics
---
