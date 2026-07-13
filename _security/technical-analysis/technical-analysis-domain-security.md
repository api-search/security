---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: technical-analysis-api.com
  spf: false
hosts:
- host: technical-analysis-api.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Technical Analysis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Technical Analysis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Technical Analysis
provider_slug: technical-analysis
slug: technical-analysis-domain-security
source_filename: technical-analysis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: technical-analysis-api.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: technical-analysis-api.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/technical-analysis/refs/heads/main/security/technical-analysis-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Cryptocurrency
- Public APIs
---
