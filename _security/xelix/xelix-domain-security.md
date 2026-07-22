---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xelix.com
  spf: true
hosts:
- cert_expires: Sep  4 10:05:05 2026 GMT
  host: xelix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xelix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xelix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xelix
provider_slug: xelix
slug: xelix-domain-security
source_filename: xelix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xelix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 10:05:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xelix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xelix/refs/heads/main/security/xelix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Accounts Payable
- Financial Technology
- Artificial Intelligence
- Fraud Prevention
- Invoice Processing
- Vendor Management
- Procure-to-Pay
- Reconciliation
---
