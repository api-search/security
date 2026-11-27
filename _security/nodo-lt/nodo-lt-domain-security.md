---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nodo.lt
  spf: true
hosts:
- cert_expires: Jan 20 17:50:41 2027 GMT
  host: nodo.lt
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nodo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nodo
provider_slug: nodo-lt
slug: nodo-lt-domain-security
source_filename: nodo-lt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nodo.lt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 17:50:41 2027 GMT\n  hsts: false\ndomains:\n- domain: nodo.lt\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nodo-lt/security/nodo-lt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Legal Tech
- Lithuanian
- MCP
- Open Data
---
