---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simplepractice.com
  spf: true
hosts:
- cert_expires: Aug 26 21:16:52 2026 GMT
  host: www.simplepractice.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simplepractice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimplePractice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SimplePractice
provider_slug: simplepractice
slug: simplepractice-domain-security
source_filename: simplepractice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simplepractice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 21:16:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: simplepractice.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplepractice/refs/heads/main/security/simplepractice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Behavioral Health
- Mental Health
- EHR
- Practice Management
- Healthcare
- Scheduling
- Telehealth
- HIPAA
- Partner API
- No Public API
---
