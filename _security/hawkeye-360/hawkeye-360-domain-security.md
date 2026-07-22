---
description: ''
domains:
- caa:
  - 0 issue "letsencypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: he360.com
  spf: true
hosts:
- cert_expires: Aug 16 12:15:24 2026 GMT
  host: www.he360.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hawkeye 360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HawkEye 360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HawkEye 360
provider_slug: hawkeye-360
slug: hawkeye-360-domain-security
source_filename: hawkeye-360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.he360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 12:15:24 2026 GMT\n  hsts: null\ndomains:\n- domain: he360.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawkeye-360/refs/heads/main/security/hawkeye-360-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- RF Geolocation
- Radio Frequency Intelligence
- Signals Intelligence
- Geospatial Intelligence
- Satellite
- Smallsat Constellation
- Space
- Maritime Domain Awareness
- Defense
- Intelligence
- National Security
- Spectrum Monitoring
- RFGeo
- RFIQ
- Mission Space
---
