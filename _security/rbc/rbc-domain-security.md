---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rbc.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rbcroyalbank.com
  spf: true
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: www.rbc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: developer.rbc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: www.rbcroyalbank.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rbc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Royal Bank of Canada, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Royal Bank of Canada
provider_slug: rbc
slug: rbc-domain-security
source_filename: rbc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rbc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\n- host: developer.rbc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\n- host: www.rbcroyalbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rbc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rbcroyalbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rbc/refs/heads/main/security/rbc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial-Services
- Banking
- Canada
- Big Six
- Payments
- Interac
- Open Banking
- Developer Portal
---
