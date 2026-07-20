---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boosted.ai
  spf: true
hosts:
- cert_expires: Aug 25 05:38:42 2026 GMT
  host: www.boosted.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 18:43:39 2026 GMT
  host: alfa.boosted.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boosted Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boosted.ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Boosted.ai
provider_slug: boosted
slug: boosted-domain-security
source_filename: boosted-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boosted.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:38:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: alfa.boosted.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:43:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: boosted.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boosted/refs/heads/main/security/boosted-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Finance
- Investment Management
- Financial Services
- Agents
- Machine Learning
- Research
- Fintech
---
