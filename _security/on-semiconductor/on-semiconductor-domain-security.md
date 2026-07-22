---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onsemi.com
  spf: true
hosts:
- cert_expires: Aug  9 11:02:51 2026 GMT
  host: www.onsemi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: On Semiconductor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for onsemi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: onsemi
provider_slug: on-semiconductor
slug: on-semiconductor-domain-security
source_filename: on-semiconductor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onsemi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 11:02:51 2026 GMT\n  hsts: null\ndomains:\n- domain: onsemi.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/on-semiconductor/refs/heads/main/security/on-semiconductor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Semiconductors
- Power Management
- Image Sensing
- Automotive
- Industrial
- Fortune 1000
---
