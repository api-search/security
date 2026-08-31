---
description: ''
domains:
- a: []
  aaaa: []
  caa: []
  creation_date: '2005-07-11'
  dmarc: false
  dmarc_policy: null
  dnskey: []
  dnssec: false
  domain: flightcar.com
  mx: []
  nameservers:
  - 1-ceci.njalla.do.
  - 2-nest.pipe.ma.
  - 3-pas.njalla.in.
  registrar: Tucows Domains Inc.
  registry_expiry: '2028-07-11'
  soa: 1-ceci.njalla.do. you.can-get-no.info. 2026071813
  spf: false
  status:
  - clientTransferProhibited
  - clientUpdateProhibited
  whois_updated: '2026-07-18'
hosts:
- curl_exit: could-not-connect
  host: flightcar.com
  hsts: null
  http_status: null
  https: false
  note: no A/AAAA record; connection could not be established
  reachable: false
  tls_version: null
- curl_exit: could-not-connect
  host: www.flightcar.com
  hsts: null
  http_status: null
  https: false
  note: no A/AAAA record
  reachable: false
  tls_version: null
- host: api.flightcar.com
  https: false
  note: no DNS resolution
  reachable: false
- host: developer.flightcar.com
  https: false
  note: no DNS resolution
  reachable: false
- host: docs.flightcar.com
  https: false
  note: no DNS resolution
  reachable: false
kind: domain-security
layout: security
method: probed
name: Flightcar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlightCar, probed live across 5 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FlightCar
provider_slug: flightcar
slug: flightcar-domain-security
source_filename: flightcar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + curl probe of flightcar.com (enrichment pipeline, local pass)\nnotes: >-\n  The registrable domain flightcar.com is registered but publishes no address\n  records and serves no site. Every probe below returned an honest negative,\n  which is recorded as valid data rather than treated as a failure. Taken\n  together these are the DNS fingerprint of a parked/abandoned domain, not of a\n  live API provider.\nhosts:\n  - host: flightcar.com\n    https: false\n    reachable: false\n    http_status: null\n    curl_exit: could-not-connect\n    tls_version: null\n    hsts: null\n    note: no A/AAAA record; connection could not be established\n  - host: www.flightcar.com\n    https: false\n    reachable: false\n    http_status: null\n    curl_exit: could-not-connect\n    tls_version: null\n    hsts: null\n    note: no A/AAAA record\n  - host: api.flightcar.com\n    https: false\n    reachable: false\n    note: no DNS resolution\n\
  \  - host: developer.flightcar.com\n    https: false\n    reachable: false\n    note: no DNS resolution\n  - host: docs.flightcar.com\n    https: false\n    reachable: false\n    note: no DNS resolution\ndomains:\n  - domain: flightcar.com\n    a: []\n    aaaa: []\n    mx: []\n    dnssec: false\n    dnskey: []\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    nameservers:\n      - 1-ceci.njalla.do.\n      - 2-nest.pipe.ma.\n      - 3-pas.njalla.in.\n    soa: 1-ceci.njalla.do. you.can-get-no.info. 2026071813\n    registrar: Tucows Domains Inc.\n    creation_date: '2005-07-11'\n    registry_expiry: '2028-07-11'\n    whois_updated: '2026-07-18'\n    status:\n      - clientTransferProhibited\n      - clientUpdateProhibited\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightcar/refs/heads/main/security/flightcar-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Defunct
- Transportation
- Travel
- Automotive
- Car Rental
- Marketplace
- Peer To Peer
- Mobility
---
