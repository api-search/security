---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: principal-financial.com
  spf: false
hosts:
- host: www.principal-financial.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Principal Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for principal-financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: principal-financial
provider_slug: principal-financial
slug: principal-financial-domain-security
source_filename: principal-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.principal-financial.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: principal-financial.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/principal-financial/refs/heads/main/security/principal-financial-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Fortune 500
---
