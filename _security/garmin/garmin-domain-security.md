---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: garmin.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thisisant.com
  spf: true
hosts:
- cert_expires: Aug 20 18:31:28 2026 GMT
  host: www.garmin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 18:01:29 2026 GMT
  host: developer.garmin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 17:26:03 2026 GMT
  host: www.thisisant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Garmin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Garmin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Garmin
provider_slug: garmin
slug: garmin-domain-security
source_filename: garmin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.garmin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.garmin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:01:29 2026 GMT\n  hsts: false\n- host: www.thisisant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:26:03 2026 GMT\n  hsts: false\ndomains:\n- domain: garmin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: thisisant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garmin/refs/heads/main/security/garmin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GPS
- Fitness
- Wearables
- Outdoor
- Connect IQ
- Health
- Cycling
- Marine
- Aviation
- Automotive
- FIT
- ANT
---
