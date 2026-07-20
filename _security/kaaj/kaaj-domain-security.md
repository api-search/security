---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kaaj.ai
  spf: true
hosts:
- cert_expires: Oct  6 21:46:44 2026 GMT
  host: kaaj.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 12:03:51 2026 GMT
  host: docs.kaaj.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 06:36:45 2026 GMT
  host: api.kaaj.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaaj Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaaj, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Kaaj
provider_slug: kaaj
slug: kaaj-domain-security
source_filename: kaaj-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaaj.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:46:44 2026 GMT\n  hsts: null\n- host: docs.kaaj.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 12:03:51 2026 GMT\n  hsts: null\n- host: api.kaaj.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:36:45 2026 GMT\n  hsts: null\ndomains:\n- domain: kaaj.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaaj/refs/heads/main/security/kaaj-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Lending
- Underwriting
- Credit Risk
- Small Business
- Artificial Intelligence
- Agentic AI
- Document Intelligence
- KYB
- Fraud Detection
- Bank Statement Analysis
---
