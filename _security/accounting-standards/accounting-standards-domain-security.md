---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fasb.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ifrs.org
  spf: true
hosts:
- cert_expires: Sep  4 03:15:52 2026 GMT
  host: www.fasb.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 16:34:20 2026 GMT
  host: www.ifrs.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:03:22 2026 GMT
  host: xbrl.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accounting Standards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accounting Standards, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Accounting Standards
provider_slug: accounting-standards
slug: accounting-standards-domain-security
source_filename: accounting-standards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fasb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:15:52 2026 GMT\n  hsts: null\n- host: www.ifrs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 16:34:20 2026 GMT\n  hsts: false\n- host: xbrl.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:03:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fasb.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ifrs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accounting-standards/refs/heads/main/security/accounting-standards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting Standards
- Finance
- GAAP
- IFRS
- XBRL
- Financial Reporting
- SEC
- FASB
---
