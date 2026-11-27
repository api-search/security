---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: minutaia.com.br
  spf: true
hosts:
- cert_expires: Feb  8 14:58:54 2027 GMT
  host: minutaia.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MinutaIA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MinutaIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MinutaIA
provider_slug: minutaia-com-br
slug: minutaia-com-br-domain-security
source_filename: minutaia-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minutaia.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 14:58:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: minutaia.com.br\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/minutaia-com-br/security/minutaia-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Artificial Intelligence
- Brazil
- Software-as-a-Service
- Document Automation
- Company
---
