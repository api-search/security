---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hopgraph.com
  spf: true
hosts:
- cert_expires: Jan 25 20:37:42 2027 GMT
  host: hopgraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: hopgraph-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hopgraph-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: hopgraph-com
provider_slug: hopgraph-com
slug: hopgraph-com-domain-security
source_filename: hopgraph-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hopgraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 20:37:42 2027 GMT\n  hsts: null\ndomains:\n- domain: hopgraph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hopgraph-com/security/hopgraph-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Business Verification
- Compliance
- Government Data
- Monitoring
---
