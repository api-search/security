---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@yahooinc.com"
  - 0 issue ";"
  dmarc: false
  dnssec: false
  domain: incredible.io
  spf: false
hosts:
- host: incredible.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''incredible.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Incredible Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Don.na, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Don.na
provider_slug: incredible-io
slug: incredible-io-domain-security
source_filename: incredible-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incredible.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''incredible.'\n  hsts: null\ndomains:\n- domain: incredible.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@yahooinc.com\"\n  - 0 issue \";\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/incredible-io/security/incredible-io-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Startup
- Technology
- API
- Venture
---
