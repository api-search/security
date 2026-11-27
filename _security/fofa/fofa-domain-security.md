---
description: ''
domains:
- caa:
  - fofa.info.cdn.cloudflare.net.
  dmarc: false
  dnssec: true
  domain: fofa.info
  spf: false
hosts:
- cert_expires: Jan  6 17:04:47 2027 GMT
  host: fofa.info
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FOFA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FOFA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: FOFA
provider_slug: fofa
slug: fofa-domain-security
source_filename: fofa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fofa.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 17:04:47 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: fofa.info\n  dnssec: true\n  caa:\n  - fofa.info.cdn.cloudflare.net.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fofa/security/fofa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Cybersecurity
- Search Engines
- Threat Intelligence
- Asset Discovery
---
