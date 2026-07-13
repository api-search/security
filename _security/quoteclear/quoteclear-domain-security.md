---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: web.app
  spf: false
hosts:
- cert_expires: Aug 18 17:14:16 2026 GMT
  host: quoteclear.web.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quoteclear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for quoteclear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: quoteclear
provider_slug: quoteclear
slug: quoteclear-domain-security
source_filename: quoteclear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quoteclear.web.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:14:16 2026 GMT\n  hsts: null\ndomains:\n- domain: web.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quoteclear/refs/heads/main/security/quoteclear-domain-security.yml
summary_line: TLSv1.3
tags:
- Personality
- Public APIs
---
