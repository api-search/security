---
description: ''
domains:
- caa:
  - 0 issue "emudhra.com"
  - 0 issue "emsign.com"
  - 0 issue "amazon.com"
  - 0 issue "ssl.com"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nyu.edu
  spf: true
hosts:
- host: nyu.edu
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1147)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: New York University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New York University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: New York University
provider_slug: nyu-edu
slug: nyu-edu-domain-security
source_filename: nyu-edu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nyu.edu\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1147)'\n  hsts: null\ndomains:\n- domain: nyu.edu\n  dnssec: false\n  caa:\n  - 0 issue \"emudhra.com\"\n  - 0 issue \"emsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nyu-edu/security/nyu-edu-domain-security.yml
summary_line: DMARC
tags:
- University
- Education
- Research
- New York
- Higher Education
---
