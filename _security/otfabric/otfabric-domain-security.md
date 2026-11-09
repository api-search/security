---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: otfabric.io
  spf: true
hosts:
- cert_expires: Jan 31 00:36:19 2027 GMT
  host: otfabric.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Otfabric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OT Fabric, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OT Fabric
provider_slug: otfabric
slug: otfabric-domain-security
source_filename: otfabric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: otfabric.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 00:36:19 2027 GMT\n  hsts: false\ndomains:\n- domain: otfabric.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/otfabric/security/otfabric-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial IoT
- Operational Technology
- Open Source
- Protocol
- Modbus
- OPC UA
- Go
- CLI
- Interoperability Testing
---
