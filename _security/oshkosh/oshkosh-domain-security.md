---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: oshkoshcorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oshkoshdefense.com
  spf: true
hosts:
- cert_expires: Sep 11 06:44:55 2026 GMT
  host: www.oshkoshcorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 09:51:41 2026 GMT
  host: www.oshkoshdefense.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oshkosh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oshkosh, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Oshkosh
provider_slug: oshkosh
slug: oshkosh-domain-security
source_filename: oshkosh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oshkoshcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:44:55 2026 GMT\n  hsts: false\n- host: www.oshkoshdefense.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 09:51:41 2026 GMT\n  hsts: false\ndomains:\n- domain: oshkoshcorp.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n- domain: oshkoshdefense.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oshkosh/refs/heads/main/security/oshkosh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Defense
- Fortune 500
- Industrial
- Manufacturing
- Vehicles
---
