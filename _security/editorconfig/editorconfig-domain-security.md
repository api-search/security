---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: editorconfig.org
  spf: true
hosts:
- cert_expires: Aug 31 09:03:21 2026 GMT
  host: editorconfig.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Editorconfig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EditorConfig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EditorConfig
provider_slug: editorconfig
slug: editorconfig-domain-security
source_filename: editorconfig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: editorconfig.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:03:21 2026 GMT\n  hsts: false\ndomains:\n- domain: editorconfig.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/editorconfig/refs/heads/main/security/editorconfig-domain-security.yml
summary_line: TLSv1.3
tags:
- Coding Standards
- Configuration
- Developer Tools
- File Format
- Formatting
- IDE
- Specification
---
