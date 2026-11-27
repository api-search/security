---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: beyourspace.es
  spf: true
hosts:
- cert_expires: Jan  4 08:05:07 2027 GMT
  host: beyourspace.es
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: beyourspace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for beyourspace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: beyourspace
provider_slug: beyourspace-es
slug: beyourspace-es-domain-security
source_filename: beyourspace-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beyourspace.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 08:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: beyourspace.es\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/beyourspace-es/security/beyourspace-es-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Catalog
- Pay-per-use
- Automation
- Discovery
- Spanish
---
