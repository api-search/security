---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axoni.com
  spf: true
hosts:
- cert_expires: Aug 23 11:33:35 2026 GMT
  host: axoni.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axoni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axoni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axoni
provider_slug: axoni
slug: axoni-domain-security
source_filename: axoni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axoni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:33:35 2026 GMT\n  hsts: false\ndomains:\n- domain: axoni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axoni/refs/heads/main/security/axoni-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Capital Markets
- Post-Trade
- Data Infrastructure
- Data Replication
- Fintech
- Distributed Ledger
---
