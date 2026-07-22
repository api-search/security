---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: silagroup.co.in
  spf: true
hosts:
- cert_expires: Sep 26 03:45:11 2026 GMT
  host: silagroup.co.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silagroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silagroup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Silagroup
provider_slug: silagroup
slug: silagroup-domain-security
source_filename: silagroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silagroup.co.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:45:11 2026 GMT\n  hsts: false\ndomains:\n- domain: silagroup.co.in\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silagroup/refs/heads/main/security/silagroup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Business Services
- Real Estate
- Facility Management
- Material Handling
- Food & Catering
- Real Estate Advisory
- Real Estate Development
- India
---
