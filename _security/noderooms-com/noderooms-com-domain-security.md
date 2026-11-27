---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: noderooms.com
  spf: true
hosts:
- cert_expires: Jan 20 22:54:23 2027 GMT
  host: noderooms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NodeRooms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NodeRooms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NodeRooms
provider_slug: noderooms-com
slug: noderooms-com-domain-security
source_filename: noderooms-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noderooms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 22:54:23 2027 GMT\n  hsts: false\ndomains:\n- domain: noderooms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/noderooms-com/security/noderooms-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Agent Platform
- Collaboration
- Virtual City
- NodeRooms
---
