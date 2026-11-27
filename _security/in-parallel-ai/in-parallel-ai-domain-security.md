---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: in-parallel.ai
  spf: true
hosts:
- cert_expires: Feb  3 06:04:10 2027 GMT
  host: in-parallel.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: In Parallel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for In Parallel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: In Parallel
provider_slug: in-parallel-ai
slug: in-parallel-ai-domain-security
source_filename: in-parallel-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: in-parallel.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 06:04:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: in-parallel.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/in-parallel-ai/security/in-parallel-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Collaboration
- Artificial Intelligence
- Productivity
- Software-as-a-Service
- Teamwork
---
