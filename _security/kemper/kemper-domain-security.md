---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kemper.com
  spf: true
hosts:
- cert_expires: Sep 25 00:41:33 2026 GMT
  host: www.kemper.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kemper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kemper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kemper
provider_slug: kemper
slug: kemper-domain-security
source_filename: kemper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kemper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 00:41:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kemper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kemper/refs/heads/main/security/kemper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Auto Insurance
- Life Insurance
- Financial Services
- Fortune 1000
---
