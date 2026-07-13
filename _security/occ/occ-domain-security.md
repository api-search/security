---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: treas.gov
  spf: true
- caa:
  - 128 iodef "mailto:dns-admin@occ.treas.gov"
  - 128 issue "entrust.net"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: occ.gov
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.occ.treas.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: apps.occ.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Occ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Office of the Comptroller of the Currency (OCC), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Office of the Comptroller of the Currency (OCC)
provider_slug: occ
slug: occ-domain-security
source_filename: occ-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.occ.treas.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apps.occ.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: treas.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: occ.gov\n  dnssec: true\n  caa:\n  - 128 iodef \"mailto:dns-admin@occ.treas.gov\"\n  - 128 issue \"entrust.net\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/occ/refs/heads/main/security/occ-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Federal
- Regulation
- National Banks
- Financial Institutions
- CRA
- Enforcement
- Licensing
---
