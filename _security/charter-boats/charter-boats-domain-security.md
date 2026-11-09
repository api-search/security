---
api_specs:
- filename: charter-boats-openapi-generated.yml
  format: yaml
  label: Charter Boats API
  slug: charter-boats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/charter-boats/openapi/_ae-authored/charter-boats-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charter.boats
  spf: true
hosts:
- cert_expires: Jan 11 00:19:41 2027 GMT
  host: charter.boats
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Charter Boats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charter Boats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Charter Boats
provider_slug: charter-boats
slug: charter-boats-domain-security
source_filename: charter-boats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: charter.boats\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 00:19:41 2027 GMT\n  hsts: false\ndomains:\n- domain: charter.boats\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/charter-boats/security/charter-boats-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sailing
- Charter
- Boats
- Travel
---
