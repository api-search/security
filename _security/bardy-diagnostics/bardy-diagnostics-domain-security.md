---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bardydx.com
  spf: true
hosts:
- cert_expires: Nov 25 20:06:43 2026 GMT
  host: www.bardydx.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bardy Diagnostics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bardy Diagnostics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bardy Diagnostics
provider_slug: bardy-diagnostics
slug: bardy-diagnostics-domain-security
source_filename: bardy-diagnostics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bardydx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: bardydx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bardy-diagnostics/refs/heads/main/security/bardy-diagnostics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Cardiology
- Diagnostics
- RemoteMonitoring
---
