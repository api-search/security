---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: demovela.com
  spf: false
hosts:
- cert_expires: Dec 20 16:26:38 2026 GMT
  host: demovela.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Demovela Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Demovela, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Demovela
provider_slug: demovela-com
slug: demovela-com-domain-security
source_filename: demovela-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: demovela.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 16:26:38 2026 GMT\n  hsts: false\ndomains:\n- domain: demovela.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/demovela-com/security/demovela-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Video
- Product Demos
- Marketing Video
- Video Generation
- MCP
- n8n
- Software-as-a-Service
---
