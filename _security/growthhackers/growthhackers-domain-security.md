---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: growthhackers.com
  spf: true
hosts:
- cert_expires: Sep 19 07:54:59 2026 GMT
  host: growthhackers.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Growthhackers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GrowthHackers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GrowthHackers
provider_slug: growthhackers
slug: growthhackers-domain-security
source_filename: growthhackers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: growthhackers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:54:59 2026 GMT\n  hsts: null\ndomains:\n- domain: growthhackers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthhackers/refs/heads/main/security/growthhackers-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Community
- Growth Hacking
- Marketing
---
