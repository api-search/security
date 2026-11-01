---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dstzc.com
  spf: false
hosts:
- host: dstzc.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''dstzc.com''.'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dstzc Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dstzc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: dstzc
provider_slug: dstzc-com
slug: dstzc-com-domain-security
source_filename: dstzc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dstzc.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''dstzc.com''.'\n  hsts: null\ndomains:\n- domain: dstzc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dstzc-com/security/dstzc-com-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Logistics
- Electric Vehicles
- China
- Transportation
- Technology
---
