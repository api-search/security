---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flownode.io
  spf: false
hosts:
- cert_expires: Dec 25 09:03:28 2026 GMT
  host: flownode.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlowNode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlowNode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FlowNode
provider_slug: flownode-io
slug: flownode-io-domain-security
source_filename: flownode-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flownode.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 09:03:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: flownode.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flownode-io/security/flownode-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Creative Platform
- NodeBased
- Studio
---
