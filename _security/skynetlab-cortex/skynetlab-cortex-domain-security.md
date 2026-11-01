---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: skynetlab-cortex.com
  spf: true
hosts:
- cert_expires: Dec 21 20:33:56 2026 GMT
  host: skynetlab-cortex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skynetlab Cortex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SKYNETLAB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SKYNETLAB
provider_slug: skynetlab-cortex
slug: skynetlab-cortex-domain-security
source_filename: skynetlab-cortex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skynetlab-cortex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 20:33:56 2026 GMT\n  hsts: false\ndomains:\n- domain: skynetlab-cortex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/skynetlab-cortex/security/skynetlab-cortex-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- SemanticMemory
- ChatGPTConnector
- Infrastructure
---
