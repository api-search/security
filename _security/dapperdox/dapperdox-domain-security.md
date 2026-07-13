---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dapperdox.io
  spf: false
hosts:
- host: dapperdox.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''dapperdox.i'
kind: domain-security
layout: security
method: probed
name: Dapperdox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DapperDox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DapperDox
provider_slug: dapperdox
slug: dapperdox-domain-security
source_filename: dapperdox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dapperdox.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''dapperdox.i'\n  hsts: null\ndomains:\n- domain: dapperdox.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dapperdox/refs/heads/main/security/dapperdox-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- API Reference
- Documentation
- Developer Tools
- Open Source
- OpenAPI
- Static Site
---
