---
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: delphia.com
  spf: true
hosts:
- cert_expires: Sep 15 01:01:25 2026 GMT
  host: delphia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Delphia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delphia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Delphia
provider_slug: delphia
slug: delphia-domain-security
source_filename: delphia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delphia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:01:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: delphia.com\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delphia/refs/heads/main/security/delphia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Fintech
- Investing
- Artificial Intelligence
- Data
- Quantitative Finance
---
