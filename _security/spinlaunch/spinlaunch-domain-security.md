---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spinlaunch.com
  spf: true
hosts:
- cert_expires: Sep 21 09:22:49 2026 GMT
  host: www.spinlaunch.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spinlaunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpinLaunch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SpinLaunch
provider_slug: spinlaunch
slug: spinlaunch-domain-security
source_filename: spinlaunch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spinlaunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: spinlaunch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spinlaunch/refs/heads/main/security/spinlaunch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Frontier Tech
- Space
- Aerospace
- Satellite
- Launch Systems
- Broadband
- Space Technology
---
