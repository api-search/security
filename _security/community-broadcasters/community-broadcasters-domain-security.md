---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: commbroadcasters.com
  spf: true
hosts:
- cert_expires: Nov 21 05:48:55 2026 GMT
  host: commbroadcasters.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Community Broadcasters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Community Broadcasters, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Community Broadcasters
provider_slug: community-broadcasters
slug: community-broadcasters-domain-security
source_filename: community-broadcasters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commbroadcasters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 05:48:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: commbroadcasters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community-broadcasters/refs/heads/main/security/community-broadcasters-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
