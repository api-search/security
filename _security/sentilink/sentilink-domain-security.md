---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sentilink.com
  spf: true
hosts:
- cert_expires: Sep 30 08:28:16 2026 GMT
  host: www.sentilink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.sentilink.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 05:21:19 2026 GMT
  host: resources.sentilink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sentilink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SentiLink, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SentiLink
provider_slug: sentilink
slug: sentilink-domain-security
source_filename: sentilink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sentilink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:28:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sentilink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\n- host: resources.sentilink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:21:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sentilink.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentilink/refs/heads/main/security/sentilink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Detection
- Identity Verification
- Synthetic Identity
- Account Takeover
- First-Party Fraud
- Financial Services
- Risk Scoring
- Fintech
- KYC
- AML
---
