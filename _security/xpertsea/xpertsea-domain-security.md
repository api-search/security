---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bekampi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xpertsea.com
  spf: true
hosts:
- cert_expires: Sep  5 05:08:39 2026 GMT
  host: bekampi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:28:15 2026 GMT
  host: www.xpertsea.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xpertsea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xpertsea, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xpertsea
provider_slug: xpertsea
slug: xpertsea-domain-security
source_filename: xpertsea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bekampi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:08:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.xpertsea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:28:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bekampi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: xpertsea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xpertsea/refs/heads/main/security/xpertsea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Aquaculture
- Shrimp Farming
- Agriculture Technology
- Artificial Intelligence
- Mobile Applications
---
