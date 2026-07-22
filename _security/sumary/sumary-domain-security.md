---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@sumary.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sumary.com
  spf: true
hosts:
- cert_expires: Oct 15 03:58:35 2026 GMT
  host: sumary.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sumary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sumary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sumary
provider_slug: sumary
slug: sumary-domain-security
source_filename: sumary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sumary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 03:58:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sumary.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@sumary.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumary/refs/heads/main/security/sumary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Fintech
- Accounting
- Automation
- Artificial Intelligence
- Anomaly Detection
- Denmark
---
