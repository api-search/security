---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cityblock.com
  spf: true
hosts:
- cert_expires: Oct 10 19:07:14 2026 GMT
  host: cityblock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City Block Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City Block, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: City Block
provider_slug: city-block
slug: city-block-domain-security
source_filename: city-block-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cityblock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:07:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cityblock.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-block/refs/heads/main/security/city-block-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Value-Based Care
- Medicaid
- Behavioral Health
- Primary Care
- Care Coordination
- Digital Health
---
