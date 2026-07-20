---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fountain.com
  spf: true
hosts:
- cert_expires: Oct  2 19:55:41 2026 GMT
  host: developer.fountain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 16:30:35 2026 GMT
  host: services.fountain.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fountain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fountain, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fountain
provider_slug: fountain
slug: fountain-domain-security
source_filename: fountain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.fountain.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 19:55:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.fountain.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 16:30:35 2026 GMT\n  hsts: null\ndomains:\n- domain: fountain.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fountain/refs/heads/main/security/fountain-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Enterprise
- Hiring
- Recruiting
- Applicant Tracking
- Human Resources
- Workforce Management
- Onboarding
- Scheduling
- HR Tech
- Frontline
---
