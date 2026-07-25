---
description: ''
domains:
- caa:
  - 1 issuewild "digicert.com"
  - 1 issue "digicert.com"
  - 1 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rbfcu.org
  spf: true
hosts:
- cert_expires: Aug  2 23:59:59 2026 GMT
  host: www.rbfcu.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Randolph Brooks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Randolph-Brooks FCU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Randolph-Brooks FCU
provider_slug: randolph-brooks
slug: randolph-brooks-domain-security
source_filename: randolph-brooks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rbfcu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rbfcu.org\n  dnssec: false\n  caa:\n  - 1 issuewild \"digicert.com\"\n  - 1 issue \"digicert.com\"\n  - 1 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/randolph-brooks/refs/heads/main/security/randolph-brooks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- United States
- Credit Union
- Retail Banking
- Open Finance
- Data Aggregation
---
