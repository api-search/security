---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jazzhr.com
  spf: true
hosts:
- cert_expires: Dec  5 14:41:58 2026 GMT
  host: www.jazzhr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jazzhr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JazzHR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: JazzHR
provider_slug: jazzhr
slug: jazzhr-domain-security
source_filename: jazzhr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jazzhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 14:41:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jazzhr.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jazzhr/refs/heads/main/security/jazzhr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Recruiting
- Applicant Tracking
- Small Business
- Hiring
- Software-as-a-Service
- Company
---
