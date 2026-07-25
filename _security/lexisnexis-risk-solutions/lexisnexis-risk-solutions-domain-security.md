---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lexisnexis.com
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issue "vikingcloud.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lexisnexisrisk.com
  spf: true
hosts:
- cert_expires: Dec 11 21:06:20 2026 GMT
  host: risk.lexisnexis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 16:12:53 2026 GMT
  host: developer.lexisnexisrisk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lexisnexis Risk Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LexisNexis Risk Solutions, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LexisNexis Risk Solutions
provider_slug: lexisnexis-risk-solutions
slug: lexisnexis-risk-solutions-domain-security
source_filename: lexisnexis-risk-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: risk.lexisnexis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 21:06:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lexisnexisrisk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:12:53 2026 GMT\n  hsts: false\ndomains:\n- domain: lexisnexis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lexisnexisrisk.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"vikingcloud.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexisnexis-risk-solutions/refs/heads/main/security/lexisnexis-risk-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- United States
- Risk Data
- Property and Casualty
- Underwriting
- Claims
- Life Insurance
- Auto Insurance
- Data Analytics
- Partner Gated
---
