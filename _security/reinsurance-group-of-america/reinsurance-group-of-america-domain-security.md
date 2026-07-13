---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rgare.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rgax.com
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: www.rgare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: www.rgax.com
  https: false
- cert_expires: Oct  1 20:27:57 2026 GMT
  host: investor.rgare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reinsurance Group Of America Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reinsurance Group of America, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reinsurance Group of America
provider_slug: reinsurance-group-of-america
slug: reinsurance-group-of-america-domain-security
source_filename: reinsurance-group-of-america-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rgare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.rgax.com\n  https: false\n- host: investor.rgare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:27:57 2026 GMT\n  hsts: null\ndomains:\n- domain: rgare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rgax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reinsurance-group-of-america/refs/heads/main/security/reinsurance-group-of-america-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial Services
- Health Insurance
- Insurance Technology
- Life Insurance
- Reinsurance
- Underwriting
- Fortune 500
---
