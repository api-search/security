---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: borgwarner.com
  spf: true
hosts:
- cert_expires: Sep 11 14:42:43 2026 GMT
  host: www.borgwarner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Borgwarner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BorgWarner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BorgWarner
provider_slug: borgwarner
slug: borgwarner-domain-security
source_filename: borgwarner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.borgwarner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:42:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: borgwarner.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/borgwarner/refs/heads/main/security/borgwarner-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Connected Vehicles
- Clean Mobility
- Electric Vehicles
- Propulsion Systems
- Fortune 500
---
