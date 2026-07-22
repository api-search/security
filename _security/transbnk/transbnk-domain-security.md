---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transbnk.co.in
  spf: true
hosts:
- cert_expires: Sep 22 12:50:23 2026 GMT
  host: transbnk.co.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transbnk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transbnk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Transbnk
provider_slug: transbnk
slug: transbnk-domain-security
source_filename: transbnk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transbnk.co.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:50:23 2026 GMT\n  hsts: null\ndomains:\n- domain: transbnk.co.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transbnk/refs/heads/main/security/transbnk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Transaction Banking
- Corporate Banking
- Open Finance
- Embedded Finance
- Escrow
- Payments
- Banking Infrastructure
- India
---
