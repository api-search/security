---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qerjagroup.com
  spf: true
hosts:
- host: qerjagroup.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''qerjagroup.'
kind: domain-security
layout: security
method: probed
name: Qerja Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qerja, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Qerja
provider_slug: qerja
slug: qerja-domain-security
source_filename: qerja-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qerjagroup.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''qerjagroup.'\n  hsts: null\ndomains:\n- domain: qerjagroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qerja/refs/heads/main/security/qerja-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Human Resources
- Recruitment
- Jobs
- HR Technology
- Indonesia
---
