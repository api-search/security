---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cistadesign.com
  spf: true
hosts:
- host: www.cistadesign.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.cistade'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cista Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cista, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cista
provider_slug: cista
slug: cista-domain-security
source_filename: cista-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cistadesign.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.cistade'\n  hsts: null\ndomains:\n- domain: cistadesign.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cista/security/cista-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Vision
- Imaging
- Sensors
- Semiconductor
- Technology
---
