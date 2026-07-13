---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ally.com
  spf: true
hosts:
- host: developer.ally.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''developer.a'
- host: api.ally.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ally Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ALLY Financial, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ALLY Financial
provider_slug: ally-financial
slug: ally-financial-domain-security
source_filename: ally-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.ally.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''developer.a'\n  hsts: null\n- host: api.ally.com\n  https: false\ndomains:\n- domain: ally.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ally-financial/refs/heads/main/security/ally-financial-domain-security.yml
summary_line: DMARC
tags:
- Fortune 500
---
