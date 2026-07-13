---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fountain.com
  spf: true
hosts:
- cert_expires: Sep 16 20:56:30 2026 GMT
  host: www.fountain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:55:41 2026 GMT
  host: developer.fountain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 16:30:35 2026 GMT
  host: services.fountain.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fountain Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fountain, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fountain
provider_slug: fountain-tech
slug: fountain-tech-domain-security
source_filename: fountain-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fountain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:56:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.fountain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:55:41 2026 GMT\n  hsts: null\n- host: services.fountain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 16:30:35 2026 GMT\n  hsts: null\ndomains:\n- domain: fountain.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fountain-tech/refs/heads/main/security/fountain-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hiring
- Recruiting
- Onboarding
- Applicant Tracking
- Workforce Management
- Hourly Workers
- Frontline
- Shift Management
- Scheduling
- Background Checks
- I-9 Verification
- Webhooks
- HRIS
- Talent Acquisition
- AI Agents
---
