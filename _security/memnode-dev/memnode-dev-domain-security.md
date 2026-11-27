---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: memnode.dev
  spf: true
hosts:
- cert_expires: Jan 12 00:40:22 2027 GMT
  host: memnode.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: memnode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for memnode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: memnode
provider_slug: memnode-dev
slug: memnode-dev-domain-security
source_filename: memnode-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memnode.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 00:40:22 2027 GMT\n  hsts: false\ndomains:\n- domain: memnode.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/memnode-dev/security/memnode-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Memory
- Agents
- Platform
---
