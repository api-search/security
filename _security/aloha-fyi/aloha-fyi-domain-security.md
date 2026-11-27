---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aloha.fyi
  spf: true
hosts:
- cert_expires: Dec 15 02:07:29 2026 GMT
  host: aloha.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ALOHA.FYI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ALOHA.FYI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ALOHA.FYI
provider_slug: aloha-fyi
slug: aloha-fyi-domain-security
source_filename: aloha-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aloha.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 02:07:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aloha.fyi\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aloha-fyi/security/aloha-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tours
- Activities
- AI Concierge
---
