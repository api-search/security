---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: af.mil
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airforce.com
  spf: true
hosts:
- cert_expires: Aug 30 15:46:40 2026 GMT
  host: www.afrc.af.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: www.airforce.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: mypers.af.mil
  https: false
kind: domain-security
layout: security
method: probed
name: Air Force Reserve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Air Force Reserve, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Air Force Reserve
provider_slug: air-force-reserve
slug: air-force-reserve-domain-security
source_filename: air-force-reserve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afrc.af.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:46:40 2026 GMT\n  hsts: null\n- host: www.airforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mypers.af.mil\n  https: false\ndomains:\n- domain: af.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: airforce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/air-force-reserve/refs/heads/main/security/air-force-reserve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Military
- Defense
- Air Force
- United States Government
---
