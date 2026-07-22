---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fairbanc.app
  spf: true
hosts:
- host: fairbanc.app
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Fairbanc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fairbanc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fairbanc
provider_slug: fairbanc
slug: fairbanc-domain-security
source_filename: fairbanc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fairbanc.app\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: fairbanc.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fairbanc/refs/heads/main/security/fairbanc-domain-security.yml
summary_line: DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- Buy Now Pay Later
- Embedded Finance
- Supply Chain Finance
- SME Financing
- Indonesia
---
