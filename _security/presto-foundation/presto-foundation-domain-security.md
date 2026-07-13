---
api_specs:
- filename: presto-foundation-openapi.yml
  format: yaml
  label: Presto Client REST API
  slug: presto-client-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/openapi/presto-foundation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prestodb.io
  spf: true
hosts:
- cert_expires: Sep 30 18:01:38 2026 GMT
  host: prestodb.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Presto Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Presto Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Presto Foundation
provider_slug: presto-foundation
slug: presto-foundation-domain-security
source_filename: presto-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prestodb.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:01:38 2026 GMT\n  hsts: null\ndomains:\n- domain: prestodb.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/presto-foundation/refs/heads/main/security/presto-foundation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Big Data
- Distributed SQL
- Linux Foundation
- Open Source
- Query Engine
- SQL
---
