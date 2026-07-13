---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "telesec.de"
  - 0 issuewild "letsencrypt.org"
  - 128 iodef "mailto:webmaster@berlinonline.net"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: berlin.de
  spf: true
hosts:
- cert_expires: Aug  5 12:51:53 2026 GMT
  host: datenregister.berlin.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datenregister Berlin De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datenregister Berlin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Datenregister Berlin
provider_slug: datenregister-berlin-de
slug: datenregister-berlin-de-domain-security
source_filename: datenregister-berlin-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datenregister.berlin.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 12:51:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: berlin.de\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"telesec.de\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 128 iodef \"mailto:webmaster@berlinonline.net\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datenregister-berlin-de/refs/heads/main/security/datenregister-berlin-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Germany
---
