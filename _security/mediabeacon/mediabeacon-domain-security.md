---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: esko.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mediabeacon.com
  spf: true
hosts:
- cert_expires: Sep 15 00:10:09 2026 GMT
  host: www.esko.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: www.mediabeacon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mediabeacon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediaBeacon, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MediaBeacon
provider_slug: mediabeacon
slug: mediabeacon-domain-security
source_filename: mediabeacon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.esko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:10:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.mediabeacon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: esko.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mediabeacon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediabeacon/refs/heads/main/security/mediabeacon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DAM
- Digital Asset Management
- Integrations
- Media
---
