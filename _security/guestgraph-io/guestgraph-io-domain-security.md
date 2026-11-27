---
api_specs:
- filename: guestgraph-io-operations-api-openapi.yml
  format: yaml
  label: guestgraph-io Operations API
  slug: guestgraph-io-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guestgraph-io/openapi/guestgraph-io-operations-api-openapi.yml
- filename: guestgraph-io-webhook-api-openapi.yml
  format: yaml
  label: guestgraph-io Webhook API
  slug: guestgraph-io-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guestgraph-io/openapi/guestgraph-io-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: guestgraph.io
  spf: true
hosts:
- cert_expires: Jan 19 02:55:22 2027 GMT
  host: guestgraph.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: guestgraph-io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for guestgraph-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: guestgraph-io
provider_slug: guestgraph-io
slug: guestgraph-io-domain-security
source_filename: guestgraph-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guestgraph.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 02:55:22 2027 GMT\n  hsts: false\ndomains:\n- domain: guestgraph.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/guestgraph-io/security/guestgraph-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Identity
- Guest Data
- Hotels
- Open Source
- Graph
---
