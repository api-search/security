---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: involve.media
  spf: true
hosts:
- cert_expires: Jan  3 03:18:28 2027 GMT
  host: involve.media
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Involve Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Involve Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Involve Media
provider_slug: involve-media
slug: involve-media-domain-security
source_filename: involve-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: involve.media\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 03:18:28 2027 GMT\n  hsts: false\ndomains:\n- domain: involve.media\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/involve-media/security/involve-media-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Digital Agency
- Web Design
- SEO
- Hosting
- Canada
---
