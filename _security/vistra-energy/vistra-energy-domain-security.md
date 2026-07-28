---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vistracorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: txu.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dynegy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ambitenergy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: homefieldenergy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: trieagleenergy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: energyharbor.com
  spf: true
hosts:
- cert_expires: Oct 21 17:18:14 2026 GMT
  host: www.vistracorp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 17:18:14 2026 GMT
  host: hub.vistracorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:43:41 2026 GMT
  host: investor.vistracorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 24 14:59:50 2026 GMT
  host: www.txu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 14:59:50 2026 GMT
  host: services.txu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.dynegy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:08:27 2026 GMT
  host: www.ambitenergy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: www.homefieldenergy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:09:01 2026 GMT
  host: www.trieagleenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 13:29:31 2026 GMT
  host: www.energyharbor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vistra Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vistra Corp, probed live across 10 host(s) and 7 registrable domain(s). 10 host(s) serve HTTPS (up to TLSv1.3); 7 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vistra Corp
provider_slug: vistra-energy
slug: vistra-energy-domain-security
source_filename: vistra-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Vistra Corp controlled host in apis.yml\nnote: >-\n  Vistra Corp publishes no API host, so every host probed here is a corporate,\n  retail-brand, investor or customer-portal web property. There are no API\n  servers to probe. Absence of a record (no CAA anywhere, no HSTS on\n  www.vistracorp.com or www.txu.com) is observed data, not a gap in the probe.\nhosts:\n- host: www.vistracorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 17:18:14 2026 GMT\n  hsts: null\n- host: hub.vistracorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 17:18:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: investor.vistracorp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 06:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.txu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 14:59:50 2026 GMT\n  hsts: null\n\
  - host: services.txu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 14:59:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.dynegy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.ambitenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:08:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.homefieldenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.trieagleenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:09:01 2026 GMT\n  hsts: false\n- host: www.energyharbor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:29:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vistracorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: txu.com\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dynegy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ambitenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: homefieldenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: trieagleenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: energyharbor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nsummary:\n  hosts_probed: 10\n  https_all: true\n  tls13_hosts: 8\n  tls12_hosts: 2\n  hsts_hosts: 7\n  hsts_absent_hosts:\n  - www.vistracorp.com\n  - www.txu.com\n  - www.trieagleenergy.com\n  domains_probed: 7\n  dnssec_domains: 0\n  caa_domains: 0\n  spf_domains: 7\n  dmarc_domains: 5\n  dmarc_enforcing_domains: 0\n  observation: >-\n    Every Vistra domain publishes SPF, none publishes CAA or enables DNSSEC, and\n    every DMARC\
  \ record found is p=none (monitor only, no enforcement). The two\n    highest-traffic customer-facing hosts, www.vistracorp.com and www.txu.com,\n    return no Strict-Transport-Security header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vistra-energy/refs/heads/main/security/vistra-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Natural Gas
- Power Generation
- Retail Energy
- Smart Metering
- Green Button
- Energy Markets
- Nuclear
- Solar
- Battery Storage
- Texas
- ERCOT
---
