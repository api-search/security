---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: insigniafinancial.com.au
  spf: true
hosts:
- host: insigniafinancial.com.au
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Insignia Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insignia Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Insignia Financial
provider_slug: insignia-financial
slug: insignia-financial-domain-security
source_filename: insignia-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insigniafinancial.com.au\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: insigniafinancial.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insignia-financial/refs/heads/main/security/insignia-financial-domain-security.yml
summary_line: DMARC
tags:
- Company
- Financial Services
- Wealth Management
- Superannuation
- Asset Management
- Financial Advice
- Australia
---
