---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 98point6.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.98point6.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 98Point6 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 98point6 Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 98point6 Technologies
provider_slug: 98point6
slug: 98point6-domain-security
source_filename: 98point6-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.98point6.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 98point6.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/98point6/refs/heads/main/security/98point6-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Telehealth
- Virtual Care
- Digital Health
- Electronic Health Records
- Clinical Decision Support
- Artificial Intelligence
- Software
---
