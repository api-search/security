---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jet2.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jet2holidays.com
  spf: true
hosts:
- cert_expires: Jan 14 06:56:20 2027 GMT
  host: www.jet2.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 06:56:20 2027 GMT
  host: www.jet2holidays.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jet2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jet2, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jet2
provider_slug: jet2
slug: jet2-domain-security
source_filename: jet2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jet2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 06:56:20 2027 GMT\n  hsts: null\n- host: www.jet2holidays.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 06:56:20 2027 GMT\n  hsts: null\ndomains:\n- domain: jet2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: jet2holidays.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jet2/refs/heads/main/security/jet2-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Low Cost Carrier
- Package Holidays
- Tour Operator
- Distribution
- Booking
- Ancillaries
- Partner Gated
---
