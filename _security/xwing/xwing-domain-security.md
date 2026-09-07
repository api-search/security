---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: xwing.com
  spf: true
hosts:
- cert_expires: Nov  8 12:59:15 2026 GMT
  host: www.xwing.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xwing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xwing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Xwing
provider_slug: xwing
slug: xwing-domain-security
source_filename: xwing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xwing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 12:59:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: xwing.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xwing/refs/heads/main/security/xwing-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Aviation
- Autonomy
- Aerospace
- Unmanned Aircraft
- Air Cargo
- Defense
- Robotics
- Acquired
---
