---
description: ''
domains:
- caa:
  - 0 issue "www.digicert.com"
  - 0 iodef "mailto:caa@tacto.ai"
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tacto.ai
  spf: true
hosts:
- cert_expires: Oct 14 06:32:08 2026 GMT
  host: tacto.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tacto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tacto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tacto
provider_slug: tacto
slug: tacto-domain-security
source_filename: tacto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tacto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:32:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tacto.ai\n  dnssec: false\n  caa:\n  - 0 issue \"www.digicert.com\"\n  - 0 iodef \"mailto:caa@tacto.ai\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tacto/refs/heads/main/security/tacto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Business Applications
- Procurement
- Supply Chain
- Manufacturing
- Artificial Intelligence
- Sourcing
- Compliance
- Germany
---
