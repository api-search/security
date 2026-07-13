---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: siriusxm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: siriusxmmedia.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.siriusxm.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 11:23:47 2026 GMT
  host: www.siriusxmmedia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: developer.pandora.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sirius Xm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sirius XM, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sirius XM
provider_slug: sirius-xm
slug: sirius-xm-domain-security
source_filename: sirius-xm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.siriusxm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: www.siriusxmmedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 11:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.pandora.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: siriusxm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: siriusxmmedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirius-xm/refs/heads/main/security/sirius-xm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Audio
- Streaming
- Radio
- Music
- Podcast
- Advertising
- Entertainment
---
