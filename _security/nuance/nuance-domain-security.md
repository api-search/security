---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  - 0 issuewild "digicert.com"
  - 0 issue "microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nuance.com
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: www.nuance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: docs.nuance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: mix.nuance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nuance
provider_slug: nuance
slug: nuance-domain-security
source_filename: nuance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nuance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nuance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: false\n- host: mix.nuance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nuance.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuance/refs/heads/main/security/nuance-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Speech Recognition
- Conversational AI
- Natural Language Understanding
- Text to Speech
- Speech Synthesis
- Voice
- Dialog
- gRPC
- Healthcare AI
---
