---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fctgl.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fcmtravel.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flightcentre.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corporatetraveler.us
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: discova.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild ";"
  - 0 iodef "mailto:abuse@flightcentre.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: envoyage.com
  note: The only domain in the group with a CAA record set, and the only one whose CAA publishes an incident-reporting address (abuse@flightcentre.com).
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tpconnects.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: whereto.com
  spf: true
hosts:
- cert_expires: Oct 14 15:17:58 2026 GMT
  entity: Flight Centre Travel Group
  host: www.fctgl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 14:04:57 2026 GMT
  entity: FCM Travel
  host: www.fcmtravel.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  entity: Flight Centre Australia
  host: www.flightcentre.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 14:42:41 2026 GMT
  entity: Corporate Traveler
  host: www.corporatetraveler.us
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  entity: Discova
  host: www.discova.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  entity: Envoyage
  host: www.envoyage.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 10:33:08 2026 GMT
  entity: WhereTo (FCTG-owned)
  host: www.whereto.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:32:41 2026 GMT
  entity: TPConnects Technologies (70% FCTG-owned)
  host: tpconnects.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  entity: TPConnects Iris API host (70% FCTG-owned)
  host: api.iris.tpconnects.com
  hsts: false
  https: true
  note: The only genuine API host in the group. Negotiates TLS 1.2 (not 1.3) and serves no HSTS header. Every path returns 401.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flight Centre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flight Centre Travel Group, probed live across 9 host(s) and 8 registrable domain(s). 9 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flight Centre Travel Group
provider_slug: flight-centre
slug: flight-centre-domain-security
source_filename: flight-centre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Flight Centre Travel Group brand host in\n  apis.yml plus the majority-owned TPConnects hosts\nnote: |\n  Absence of a record (no CAA, no DNSSEC, no HSTS) is recorded data, not a gap in\n  the probe. Flight Centre Travel Group publishes no API hosts of its own, so the\n  hosts probed are the brand web properties; api.iris.tpconnects.com is the only\n  real API host in the group and it belongs to TPConnects Technologies (70%\n  FCTG-owned).\nhosts:\n- host: www.fctgl.com\n  entity: Flight Centre Travel Group\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:17:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.fcmtravel.com\n  entity: FCM Travel\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:04:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: www.flightcentre.com.au\n  entity: Flight Centre Australia\n  https: true\n  tls_version: TLSv1.3\n\
  \  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.corporatetraveler.us\n  entity: Corporate Traveler\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 14:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: www.discova.com\n  entity: Discova\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.envoyage.com\n  entity: Envoyage\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: www.whereto.com\n  entity: WhereTo (FCTG-owned)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:33:08 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: tpconnects.com\n  entity: TPConnects Technologies (70% FCTG-owned)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:32:41 2026 GMT\n  hsts: false\n- host: api.iris.tpconnects.com\n  entity: TPConnects Iris API host (70% FCTG-owned)\n\
  \  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\n  note: The only genuine API host in the group. Negotiates TLS 1.2 (not 1.3) and\n    serves no HSTS header. Every path returns 401.\ndomains:\n- domain: fctgl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fcmtravel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: flightcentre.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: corporatetraveler.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: discova.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: envoyage.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"\
  amazon.com\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:abuse@flightcentre.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: The only domain in the group with a CAA record set, and the only one whose\n    CAA publishes an incident-reporting address (abuse@flightcentre.com).\n- domain: tpconnects.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: whereto.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nsummary:\n  hosts_probed: 9\n  https_all: true\n  tls13: 8\n  tls12: 1\n  hsts: 6\n  domains_probed: 8\n  dnssec: 2\n  caa: 1\n  spf: 8\n  dmarc: 8\n  dmarc_reject: 2\n  dmarc_quarantine: 6\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flight-centre/refs/heads/main/security/flight-centre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Australia
- Corporate Travel
- Travel Agency
- Distribution
- NDC
- Aviation
- Booking
- Hotels
- Aggregator
---
