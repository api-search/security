---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thinknum.com
  spf: true
hosts:
- cert_expires: Oct  5 05:32:09 2026 GMT
  host: thinknum.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thinknum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thinknum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Thinknum
provider_slug: thinknum
slug: thinknum-domain-security
source_filename: thinknum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thinknum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 05:32:09 2026 GMT\n  hsts: false\ndomains:\n- domain: thinknum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thinknum/refs/heads/main/security/thinknum-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Alternative Data
- Financial Data
- Investment Research
- Market Intelligence
- Web Data
- Datasets
---
