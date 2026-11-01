---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gmu.edu
  spf: true
hosts:
- host: csiss.gmu.edu
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''csiss.gmu.e'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: George Mason University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for George Mason University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: George Mason University
provider_slug: george-mason-university
slug: george-mason-university-domain-security
source_filename: george-mason-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: csiss.gmu.edu\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''csiss.gmu.e'\n  hsts: null\ndomains:\n- domain: gmu.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/george-mason-university/security/george-mason-university-domain-security.yml
summary_line: DMARC
tags:
- Research
- Spatial Information
- Academic
- Software
---
