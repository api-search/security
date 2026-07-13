---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dematic.com
  spf: true
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "entrust.net"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: honeywell.com
  spf: true
hosts:
- cert_expires: Aug 23 11:16:46 2026 GMT
  host: www.dematic.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: sps.honeywell.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 22:26:59 2026 GMT
  host: www.vanderlande.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Automated Sorting Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automated Sorting Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Automated Sorting Systems
provider_slug: automated-sorting-systems
slug: automated-sorting-systems-domain-security
source_filename: automated-sorting-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dematic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 11:16:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: sps.honeywell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: www.vanderlande.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 22:26:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dematic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: honeywell.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automated-sorting-systems/refs/heads/main/security/automated-sorting-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Automation
- Conveyor Systems
- Distribution
- E-Commerce Fulfillment
- Logistics
- Package Tracking
- Parcel Sorting
- Sorting
- Warehouse
- Warehouse Automation
---
