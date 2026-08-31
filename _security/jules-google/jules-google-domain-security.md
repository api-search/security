---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: jules.google
  spf: false
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:41 2026 GMT
  host: jules.google
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: jules.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jules Google Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jules, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jules
provider_slug: jules-google
slug: jules-google-domain-security
source_filename: jules-google-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jules.google\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:41 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: jules.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: jules.google\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jules-google/refs/heads/main/security/jules-google-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Coding Agent
- Autonomous Agent
- Asynchronous Agent
- Developer Tools
- Code Generation
- Pull Requests
- GitHub
- Gemini
- Google Labs
- Software Development Lifecycle
- DevOps
---
