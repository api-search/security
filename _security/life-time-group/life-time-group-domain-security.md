---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lifetime.life
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: www.lifetime.life
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Life Time Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Life Time Group Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Life Time Group Holdings
provider_slug: life-time-group
slug: life-time-group-domain-security
source_filename: life-time-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lifetime.life\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lifetime.life\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/life-time-group/refs/heads/main/security/life-time-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Athletic Clubs
- Fitness
- Health Clubs
- Hospitality
- Wellness
---
