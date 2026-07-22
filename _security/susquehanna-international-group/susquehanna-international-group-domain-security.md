---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  - 0 issue "thawte.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sig.com
  spf: true
hosts:
- cert_expires: Sep 18 09:52:31 2026 GMT
  host: sig.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Susquehanna International Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Susquehanna International Group (SIG), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Susquehanna International Group (SIG)
provider_slug: susquehanna-international-group
slug: susquehanna-international-group-domain-security
source_filename: susquehanna-international-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sig.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 09:52:31 2026 GMT\n  hsts: false\ndomains:\n- domain: sig.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"thawte.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/susquehanna-international-group/refs/heads/main/security/susquehanna-international-group-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Quantitative Trading
- Market Making
- Proprietary Trading
- Options
- Derivatives
- Institutional Sales
- Growth Equity
- Venture Capital
- Machine Learning
- Financial Services
---
