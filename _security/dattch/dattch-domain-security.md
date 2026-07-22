---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: weareher.com
  spf: true
hosts:
- cert_expires: Aug 24 17:38:34 2026 GMT
  host: weareher.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dattch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dattch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dattch
provider_slug: dattch
slug: dattch-domain-security
source_filename: dattch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weareher.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 17:38:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: weareher.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dattch/refs/heads/main/security/dattch-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Dating
- Social
- LGBTQ
- Community
- Mobile App
- Consumer
---
