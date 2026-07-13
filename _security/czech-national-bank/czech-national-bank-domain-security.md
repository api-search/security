---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cnb.cz
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.cnb.cz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Czech National Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Czech National Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Czech National Bank
provider_slug: czech-national-bank
slug: czech-national-bank-domain-security
source_filename: czech-national-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cnb.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cnb.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/czech-national-bank/refs/heads/main/security/czech-national-bank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Currency Exchange
- Public APIs
---
