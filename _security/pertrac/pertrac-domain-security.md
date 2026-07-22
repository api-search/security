---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pertrac.com
  spf: true
hosts:
- host: www.pertrac.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.pertrac'
kind: domain-security
layout: security
method: probed
name: Pertrac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PerTrac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PerTrac
provider_slug: pertrac
slug: pertrac-domain-security
source_filename: pertrac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pertrac.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.pertrac'\n  hsts: null\ndomains:\n- domain: pertrac.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pertrac/refs/heads/main/security/pertrac-domain-security.yml
summary_line: DMARC
tags:
- Company
- Hedge Funds
- Investment Analytics
- Financial Data
- Portfolio Management
---
