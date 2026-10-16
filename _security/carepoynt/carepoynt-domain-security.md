---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carepoynt.com
  spf: true
hosts:
- cert_expires: Dec  4 21:44:47 2026 GMT
  host: www.carepoynt.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carepoynt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carepoynt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Carepoynt
provider_slug: carepoynt
slug: carepoynt-domain-security
source_filename: carepoynt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carepoynt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 21:44:47 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: carepoynt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carepoynt/refs/heads/main/security/carepoynt-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Rewards
- Wellness
- Platform
---
