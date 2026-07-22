---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: floqast.com
  spf: true
hosts:
- cert_expires: Oct 14 18:41:24 2026 GMT
  host: floqast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Floqast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FloQast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FloQast
provider_slug: floqast
slug: floqast-domain-security
source_filename: floqast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: floqast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:41:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: floqast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/floqast/refs/heads/main/security/floqast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Accounting
- Financial Close
- Reconciliation
- Record-to-Report
- Compliance
- Artificial Intelligence
- SaaS
---
