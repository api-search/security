---
description: ''
domains:
- caa:
  - 0 issue "\"sectigo.com\""
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "\"digicert.com\""
  - 0 issuewild "\"pki.goog\""
  - 0 issuewild "\"sectigo.com\""
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: secondmeasure.com
  spf: true
hosts:
- cert_expires: Sep 26 01:23:30 2026 GMT
  host: secondmeasure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Secondmeasure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secondmeasure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Secondmeasure
provider_slug: secondmeasure
slug: secondmeasure-domain-security
source_filename: secondmeasure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secondmeasure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:23:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: secondmeasure.com\n  dnssec: false\n  caa:\n  - 0 issue \"\\\"sectigo.com\\\"\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"\\\"digicert.com\\\"\"\n  - 0 issuewild \"\\\"pki.goog\\\"\"\n  - 0 issuewild \"\\\"sectigo.com\\\"\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secondmeasure/refs/heads/main/security/secondmeasure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Alternative Data
- Consumer Transaction Data
- Analytics
- Financial Data
- Market Research
- Investment Research
- Bloomberg
---
