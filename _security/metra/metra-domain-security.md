---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: metra.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: metrarail.com
  spf: true
hosts:
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: metra.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: www.metrarail.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: gtfsapi.metrarail.com
  https: false
kind: domain-security
layout: security
method: probed
name: Metra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metra, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Metra
provider_slug: metra
slug: metra-domain-security
source_filename: metra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\n- host: www.metrarail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: null\n- host: gtfsapi.metrarail.com\n  https: false\ndomains:\n- domain: metra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: metrarail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metra/refs/heads/main/security/metra-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Chicago
- Commuter Rail
- GTFS
- Public Transportation
- Transit
---
