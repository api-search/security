---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datavisor.com
  spf: true
hosts:
- cert_expires: Sep 16 22:30:40 2026 GMT
  host: www.datavisor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datavisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataVisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataVisor
provider_slug: datavisor
slug: datavisor-domain-security
source_filename: datavisor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datavisor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:30:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datavisor.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavisor/refs/heads/main/security/datavisor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fraud Detection
- Fraud Prevention
- Anti-Money Laundering
- Financial Crime
- Risk Management
- Machine Learning
- Artificial Intelligence
- Device Intelligence
- Banking
- Payments
- Compliance
---
