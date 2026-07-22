---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: partiful.com
  spf: true
hosts:
- cert_expires: Sep 10 06:02:49 2026 GMT
  host: partiful.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Partiful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Partiful, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Partiful
provider_slug: partiful
slug: partiful-domain-security
source_filename: partiful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partiful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:02:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: partiful.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/partiful/refs/heads/main/security/partiful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Events
- Invitations
- Party Planning
- RSVP
- Social
---
