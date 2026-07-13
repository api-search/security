---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: runtime.dev
  spf: true
hosts:
- cert_expires: Sep  4 18:16:08 2026 GMT
  host: codedetectionapi.runtime.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Code Detection Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Code Detection API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Code Detection API
provider_slug: code-detection-api
slug: code-detection-api-domain-security
source_filename: code-detection-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codedetectionapi.runtime.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 18:16:08 2026 GMT\n  hsts: false\ndomains:\n- domain: runtime.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code-detection-api/refs/heads/main/security/code-detection-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Text Analysis
- Public APIs
---
