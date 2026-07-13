---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rgare.com
  spf: true
hosts:
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: www.rgare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: api.rgare.com
  https: false
kind: domain-security
layout: security
method: probed
name: Reinsurance Of America Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reinsurance Group of America, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reinsurance Group of America
provider_slug: reinsurance-of-america
slug: reinsurance-of-america-domain-security
source_filename: reinsurance-of-america-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rgare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rgare.com\n  https: false\ndomains:\n- domain: rgare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reinsurance-of-america/refs/heads/main/security/reinsurance-of-america-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Reinsurance
- Life Insurance
- Health Insurance
- Underwriting
- Financial Services
- Risk Assessment
- Digital Health
- Fortune 500
---
