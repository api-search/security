---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mtch.com
  spf: true
hosts:
- cert_expires: Aug 13 20:05:03 2026 GMT
  host: www.mtch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Match Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Match Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Match Group
provider_slug: match-group
slug: match-group-domain-security
source_filename: match-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mtch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 20:05:03 2026 GMT\n  hsts: false\ndomains:\n- domain: mtch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/match-group/refs/heads/main/security/match-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Dating
- Consumer Internet
- Social
- Mobile Apps
- Subscription
---
