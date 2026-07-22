---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: securityscorecard.com
  spf: true
hosts:
- cert_expires: Oct  8 12:51:00 2026 GMT
  host: securityscorecard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Security Scorecard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SecurityScorecard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SecurityScorecard
provider_slug: security-scorecard
slug: security-scorecard-domain-security
source_filename: security-scorecard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: securityscorecard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:51:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: securityscorecard.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/security-scorecard/refs/heads/main/security/security-scorecard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Cybersecurity
- Security Ratings
- Third-Party Risk
- Risk Management
- Attack Surface
- Compliance
---
