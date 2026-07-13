---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "wosign.com"
  - 0 issue "jprs.jp"
  - 0 issue "letsencrypt.org"
  - 0 issue "emsign.com"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cbr.ru
  spf: true
hosts:
- cert_expires: Apr 13 06:49:32 2027 GMT
  host: www.cbr.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bank Of Russia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank of Russia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bank of Russia
provider_slug: bank-of-russia
slug: bank-of-russia-domain-security
source_filename: bank-of-russia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cbr.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 13 06:49:32 2027 GMT\n  hsts: false\ndomains:\n- domain: cbr.ru\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"wosign.com\"\n  - 0 issue \"jprs.jp\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"emsign.com\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-russia/refs/heads/main/security/bank-of-russia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency Exchange
- Public APIs
---
