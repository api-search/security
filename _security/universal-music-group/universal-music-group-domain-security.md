---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: universalmusic.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: Reject
  dnssec: false
  domain: umgroyalty.com
  spf: false
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: www.universalmusic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: umgroyalty.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: umpgwindow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Universal Music Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universal Music Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Universal Music Group
provider_slug: universal-music-group
slug: universal-music-group-domain-security
source_filename: universal-music-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.universalmusic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: umgroyalty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\n- host: umpgwindow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: universalmusic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: umgroyalty.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: Reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universal-music-group/refs/heads/main/security/universal-music-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Licensing
- Big Three
- Catalog
- Entertainment
- Generative Music
- Licensing
- Major Label
- Merchandising
- Music
- Music Publishing
- Recorded Music
- Royalties
- Streaming
---
