---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: airtel.lv
  spf: false
hosts:
- cert_expires: Aug 31 05:44:06 2026 GMT
  host: sys.airtel.lv
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airtel Ip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airtel IP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Airtel IP
provider_slug: airtel-ip
slug: airtel-ip-domain-security
source_filename: airtel-ip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sys.airtel.lv\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:44:06 2026 GMT\n  hsts: null\ndomains:\n- domain: airtel.lv\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airtel-ip/refs/heads/main/security/airtel-ip-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---
