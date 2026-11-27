---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dxbdata.io
  spf: true
hosts:
- cert_expires: Jan 26 18:59:14 2027 GMT
  host: dxbdata.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DXB Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DXB Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DXB Data
provider_slug: dxbdata-io
slug: dxbdata-io-domain-security
source_filename: dxbdata-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dxbdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 18:59:14 2027 GMT\n  hsts: false\ndomains:\n- domain: dxbdata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dxbdata-io/security/dxbdata-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Real Estate
- Artificial Intelligence
- Data
- Dubai
- MCP
---
