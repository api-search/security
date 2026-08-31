---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ourbranch.com
  spf: true
hosts:
- cert_expires: Aug 30 02:48:11 2026 GMT
  host: www.ourbranch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: docs.v2.api.ourbranch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 15:04:05 2026 GMT
  host: ourbranch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Branch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branch Insurance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Branch Insurance
provider_slug: branch
slug: branch-domain-security
source_filename: branch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ourbranch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 02:48:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.v2.api.ourbranch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n- host: ourbranch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:04:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ourbranch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branch/refs/heads/main/security/branch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Home Insurance
- Auto Insurance
- Renters Insurance
- Umbrella Insurance
- Quote to Bind
- GraphQL
- InsurTech
---
