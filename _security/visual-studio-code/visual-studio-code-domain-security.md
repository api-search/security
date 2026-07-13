---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: visualstudio.com
  spf: true
hosts:
- cert_expires: Nov 21 13:25:48 2026 GMT
  host: code.visualstudio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Visual Studio Code Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Visual Studio Code, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Visual Studio Code
provider_slug: visual-studio-code
slug: visual-studio-code-domain-security
source_filename: visual-studio-code-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: code.visualstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 13:25:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: visualstudio.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visual-studio-code/refs/heads/main/security/visual-studio-code-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Code Editor
- Developer Tools
- IDE
- Open Source
- Extension API
- Microsoft
---
