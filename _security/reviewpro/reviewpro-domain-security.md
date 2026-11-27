---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shijigroup.com
  spf: true
hosts:
- cert_expires: Jan 13 12:01:29 2027 GMT
  host: shijigroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ReviewPro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReviewPro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ReviewPro
provider_slug: reviewpro
slug: reviewpro-domain-security
source_filename: reviewpro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shijigroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 12:01:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shijigroup.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/reviewpro/security/reviewpro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Reputation Management
- Software-as-a-Service
- Reviews
---
