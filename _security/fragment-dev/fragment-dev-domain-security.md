---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fragment.dev
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: fragment.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.fragment.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fragment Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fragment, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Fragment
provider_slug: fragment-dev
slug: fragment-dev-domain-security
source_filename: fragment-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fragment.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\n- host: api.fragment.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fragment.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fragment-dev/refs/heads/main/security/fragment-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Ledger
- Double-Entry
- Accounting
- Fintech
- Payments
- Reconciliation
- GraphQL
- Balances
---
