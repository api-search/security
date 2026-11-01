---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: livelikevr.com
  spf: false
hosts:
- cert_expires: Nov 24 12:50:47 2026 GMT
  host: livelikevr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Livelikevr Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveLike, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LiveLike
provider_slug: livelikevr-com
slug: livelikevr-com-domain-security
source_filename: livelikevr-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: livelikevr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 12:50:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: livelikevr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/livelikevr-com/security/livelikevr-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
