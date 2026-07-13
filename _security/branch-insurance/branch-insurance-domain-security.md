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
- cert_expires: Sep 26 22:21:49 2026 GMT
  host: api.ourbranch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Branch Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Branch
provider_slug: branch-insurance
slug: branch-insurance-domain-security
source_filename: branch-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ourbranch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 02:48:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.v2.api.ourbranch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.ourbranch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:21:49 2026 GMT\n  hsts: false\ndomains:\n- domain: ourbranch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branch-insurance/refs/heads/main/security/branch-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Home Insurance
- Auto Insurance
- Umbrella Insurance
- Bundled Insurance
- Insurtech
- Reciprocal Exchange
- Embedded Insurance
- Quote to Bind
- GraphQL
- Partner API
- Affinity
- Mortgage
- Columbus Ohio
---
