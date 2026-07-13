---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: visualstudio.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Sep  6 13:38:08 2026 GMT
  host: marketplace.visualstudio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 19:38:54 2027 GMT
  host: visualstudio.microsoft.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Visual Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Visual Studio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Microsoft Visual Studio
provider_slug: microsoft-visual-studio
slug: microsoft-visual-studio-domain-security
source_filename: microsoft-visual-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketplace.visualstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:38:08 2026 GMT\n  hsts: null\n- host: visualstudio.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 19:38:54 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: visualstudio.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: false\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-visual-studio/refs/heads/main/security/microsoft-visual-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Extensions
- IDE
- Microsoft
- VS Code
---
