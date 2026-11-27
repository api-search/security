---
api_specs:
- filename: buildervet-au-api-openapi.yml
  format: yaml
  label: BuilderVet API API
  slug: buildervet-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildervet-au/openapi/_original/buildervet-au-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buildervet.au
  spf: true
hosts:
- cert_expires: Dec  9 16:08:17 2026 GMT
  host: buildervet.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BuilderVet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuilderVet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BuilderVet
provider_slug: buildervet-au
slug: buildervet-au-domain-security
source_filename: buildervet-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildervet.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 16:08:17 2026 GMT\n  hsts: false\ndomains:\n- domain: buildervet.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/buildervet-au/security/buildervet-au-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
