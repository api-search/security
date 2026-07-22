---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: siriusxm.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: corporate.siriusxm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sirius Xm Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sirius XM Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sirius XM Holdings
provider_slug: sirius-xm-holdings
slug: sirius-xm-holdings-domain-security
source_filename: sirius-xm-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corporate.siriusxm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: siriusxm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sirius-xm-holdings/refs/heads/main/security/sirius-xm-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Audio
- Audio Streaming
- Satellite Radio
- Podcasts
- Advertising Technology
- Music
- Entertainment
- Holding Company
- Public Company
---
