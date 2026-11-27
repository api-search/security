---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openbudget.sh
  spf: false
hosts:
- cert_expires: Jan 15 19:50:45 2027 GMT
  host: openbudget.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenBudget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenBudget, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: OpenBudget
provider_slug: openbudget-sh
slug: openbudget-sh-domain-security
source_filename: openbudget-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openbudget.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 19:50:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openbudget.sh\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openbudget-sh/security/openbudget-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Artificial Intelligence
- Personal Finance
- Banking
- Automation
---
