---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jasswiki.ch
  spf: true
hosts:
- cert_expires: Jan 30 13:47:42 2027 GMT
  host: jasswiki.ch
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JassWiki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JassWiki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: JassWiki
provider_slug: jasswiki-ch
slug: jasswiki-ch-domain-security
source_filename: jasswiki-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jasswiki.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 13:47:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: jasswiki.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/jasswiki-ch/security/jasswiki-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Swiss
- Card Games
- Culture
- Education
---
