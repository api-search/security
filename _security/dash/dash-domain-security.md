---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dash.org
  spf: true
hosts:
- cert_expires: Aug 29 16:23:23 2026 GMT
  host: www.dash.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 22:17:35 2026 GMT
  host: docs.dash.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 16:23:23 2026 GMT
  host: insight.dash.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dash, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dash
provider_slug: dash
slug: dash-domain-security
source_filename: dash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dash.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:23:23 2026 GMT\n  hsts: false\n- host: docs.dash.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 22:17:35 2026 GMT\n  hsts: false\n- host: insight.dash.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:23:23 2026 GMT\n  hsts: false\ndomains:\n- domain: dash.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dash/refs/heads/main/security/dash-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cryptocurrency
- Blockchain
- Dash
- InstantSend
- Masternode
- DashPay
- Governance
- Payments
---
