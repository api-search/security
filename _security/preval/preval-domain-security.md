---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: preval.dev
  spf: true
hosts:
- cert_expires: Jan 12 09:06:59 2027 GMT
  host: preval.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Preval Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preval, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Preval
provider_slug: preval
slug: preval-domain-security
source_filename: preval-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: preval.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 09:06:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: preval.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/preval/security/preval-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Observability
- Monitoring
- LLM
---
