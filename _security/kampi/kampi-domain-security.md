---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bekampi.com
  spf: true
hosts:
- cert_expires: Sep  5 05:08:39 2026 GMT
  host: bekampi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kampi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kampi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kampi
provider_slug: kampi
slug: kampi-domain-security
source_filename: kampi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bekampi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:08:39 2026 GMT\n  hsts: null\ndomains:\n- domain: bekampi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kampi/refs/heads/main/security/kampi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aquaculture
- Shrimp Farming
- Artificial Intelligence
- Machine Learning
- Mobile App
- Agriculture Technology
- Ecuador
---
