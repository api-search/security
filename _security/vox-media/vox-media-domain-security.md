---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: voxmedia.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coralproject.net
  spf: true
hosts:
- cert_expires: Aug 23 14:20:12 2026 GMT
  host: www.voxmedia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 07:43:50 2026 GMT
  host: docs.coralproject.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vox Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vox Media, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Vox Media
provider_slug: vox-media
slug: vox-media-domain-security
source_filename: vox-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voxmedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 14:20:12 2026 GMT\n  hsts: false\n- host: docs.coralproject.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: voxmedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n- domain: coralproject.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vox-media/refs/heads/main/security/vox-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Media
- Publishing
- News
- Comments
- Community
- Moderation
- GraphQL
---
