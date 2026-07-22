---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: traive.com.br
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: traive-prod.com
  spf: false
hosts:
- cert_expires: Aug 28 12:00:36 2026 GMT
  host: traive.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: auth.traive-prod.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Traive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traive, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Traive
provider_slug: traive
slug: traive-domain-security
source_filename: traive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: traive.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:00:36 2026 GMT\n  hsts: false\n- host: auth.traive-prod.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: traive.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: traive-prod.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/traive/refs/heads/main/security/traive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Fintech
- Credit
- Risk Analysis
- Lending
- AgTech
- Brazil
---
