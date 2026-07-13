---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: worldbank.org
  spf: true
hosts:
- cert_expires: Oct  2 11:29:58 2026 GMT
  host: datahelpdesk.worldbank.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: World Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: World Bank
provider_slug: world-bank
slug: world-bank-domain-security
source_filename: world-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datahelpdesk.worldbank.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:29:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: worldbank.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-bank/refs/heads/main/security/world-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Science And Math
- Public APIs
---
