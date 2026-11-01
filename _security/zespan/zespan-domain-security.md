---
api_specs:
- filename: zespan-openapi-generated.yml
  format: yaml
  label: Zespan API
  slug: zespan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zespan/openapi/_ae-authored/zespan-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zespan.com
  spf: true
hosts:
- cert_expires: Jan  9 15:02:03 2027 GMT
  host: zespan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zespan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zespan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Zespan
provider_slug: zespan
slug: zespan-domain-security
source_filename: zespan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zespan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 15:02:03 2027 GMT\n  hsts: false\ndomains:\n- domain: zespan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zespan/security/zespan-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Monitoring
- Reliability
- Agents
- Platform
---
