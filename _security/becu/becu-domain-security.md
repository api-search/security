---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "becu.org"
  - 0 issue "digicert.com"
  - 0 issuewild "becu.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: becu.org
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.becu.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Becu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BECU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BECU
provider_slug: becu
slug: becu-domain-security
source_filename: becu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.becu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: becu.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"becu.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"becu.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/becu/refs/heads/main/security/becu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- United States
- Credit Union
- Open Finance
- Data Aggregation
- CFPB 1033
---
