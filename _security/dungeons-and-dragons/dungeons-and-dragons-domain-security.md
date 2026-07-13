---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dnd5eapi.co
  spf: false
hosts:
- cert_expires: Aug 18 23:12:55 2026 GMT
  host: www.dnd5eapi.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dungeons And Dragons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dungeons and Dragons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dungeons and Dragons
provider_slug: dungeons-and-dragons
slug: dungeons-and-dragons-domain-security
source_filename: dungeons-and-dragons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dnd5eapi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:12:55 2026 GMT\n  hsts: false\ndomains:\n- domain: dnd5eapi.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dungeons-and-dragons/refs/heads/main/security/dungeons-and-dragons-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
