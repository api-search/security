---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: sherpahq.ai
  spf: false
hosts:
- cert_expires: Aug 28 11:18:48 2026 GMT
  host: sherpahq.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sherpa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sherpa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: sherpa
provider_slug: sherpa
slug: sherpa-domain-security
source_filename: sherpa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sherpahq.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:18:48 2026 GMT\n  hsts: false\ndomains:\n- domain: sherpahq.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sherpa/refs/heads/main/security/sherpa-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- External Workforce Management
- Vendor Management System
- Managed Service Provider
- AI Agents
- Contingent Labor
- Freelancer Management
- Staffing
- Procurement
- HR Tech
---
