---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
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
name: Her Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HER, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HER
provider_slug: her
slug: her-domain-security
source_filename: her-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weareher.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 17:38:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: weareher.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/her/refs/heads/main/security/her-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Dating
- LGBTQ
- Social
- Community
- Mobile App
---
