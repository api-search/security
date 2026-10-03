---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beeyondmedia.com
  spf: true
hosts:
- cert_expires: Nov  9 05:14:57 2026 GMT
  host: beeyondmedia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beeyond Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beeyond Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beeyond Media
provider_slug: beeyond-media
slug: beeyond-media-domain-security
source_filename: beeyond-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beeyondmedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 05:14:57 2026 GMT\n  hsts: false\ndomains:\n- domain: beeyondmedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeyond-media/refs/heads/main/security/beeyond-media-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Digital Out Of Home
- Programmatic
- MediaTech
- Company
---
