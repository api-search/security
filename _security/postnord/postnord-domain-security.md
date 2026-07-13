---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: postnord.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: developer.postnord.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postnord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostNord, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PostNord
provider_slug: postnord
slug: postnord-domain-security
source_filename: postnord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.postnord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: postnord.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postnord/refs/heads/main/security/postnord-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Tracking
- Public APIs
---
