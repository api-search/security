---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: edusignal.ai
  spf: false
hosts:
- cert_expires: Dec  8 09:16:22 2026 GMT
  host: edusignal.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EduSignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EduSignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: EduSignal
provider_slug: edusignal-ai
slug: edusignal-ai-domain-security
source_filename: edusignal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edusignal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 09:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: edusignal.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/edusignal-ai/security/edusignal-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Education
- Data
- K-12
- Open Data
- Community
---
