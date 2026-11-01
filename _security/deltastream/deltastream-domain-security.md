---
api_specs:
- filename: deltastream-openapi-generated.yml
  format: yaml
  label: DeltaStream API
  slug: deltastream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deltastream/openapi/_ae-authored/deltastream-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: deltastream.io
  spf: true
hosts:
- cert_expires: Jan 11 18:59:43 2027 GMT
  host: www.deltastream.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deltastream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeltaStream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DeltaStream
provider_slug: deltastream
slug: deltastream-domain-security
source_filename: deltastream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deltastream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 18:59:43 2027 GMT\n  hsts: false\ndomains:\n- domain: deltastream.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/deltastream/security/deltastream-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Real-Time
- Data Streaming
- Platform
---
