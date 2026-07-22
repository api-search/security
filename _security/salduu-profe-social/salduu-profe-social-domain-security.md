---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: profe.social
  spf: true
hosts:
- cert_expires: Oct  7 19:29:24 2026 GMT
  host: profe.social
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salduu Profe Social Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salduu (Profe Social), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Salduu (Profe Social)
provider_slug: salduu-profe-social
slug: salduu-profe-social-domain-security
source_filename: salduu-profe-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: profe.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:29:24 2026 GMT\n  hsts: false\ndomains:\n- domain: profe.social\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salduu-profe-social/refs/heads/main/security/salduu-profe-social-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Social
- Social Networking
- Fediverse
- Mastodon
- ActivityPub
- Education
---
