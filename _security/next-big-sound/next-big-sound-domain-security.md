---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nextbigsound.com
  mx:
  - mx0a-0051e301.pphosted.com
  - mx0b-0051e301.pphosted.com
  nameservers:
  - ns2.pandora.com
  - ns4.pandora.com
  spf: true
  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all
hosts:
- host: nextbigsound.com
  hsts: false
  http_status: 302
  https: false
  https_status: connection-refused
  redirect_to: http://amp.pandora.com
  tls_version: null
- host: www.nextbigsound.com
  https: false
  https_status: connection-refused
- host: api.nextbigsound.com
  https: false
  https_status: connection-refused
- host: developer.nextbigsound.com
  https: false
  https_status: connection-refused
kind: domain-security
layout: security
method: probed
name: Next Big Sound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Next Big Sound, probed live across 4 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Next Big Sound
provider_slug: next-big-sound
slug: next-big-sound-domain-security
source_filename: next-big-sound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + curl probe of nextbigsound.com (apis.yml Website host)\nnotes: >-\n  nextbigsound.com is no longer an independent web/API property. All hosts\n  resolve to a Pandora BigIP (199.116.162.108, nameservers ns2/ns4.pandora.com)\n  and HTTPS is refused on every host; HTTP/80 returns 302 -> http://amp.pandora.com\n  (Pandora Artist Marketing Platform, the successor to Next Big Sound). Only the\n  mail/DNS surface remains active. Absence of records below is real, recorded data.\nhosts:\n  - host: nextbigsound.com\n    https: false\n    https_status: connection-refused\n    tls_version: null\n    hsts: false\n    http_status: 302\n    redirect_to: http://amp.pandora.com\n  - host: www.nextbigsound.com\n    https: false\n    https_status: connection-refused\n  - host: api.nextbigsound.com\n    https: false\n    https_status: connection-refused\n  - host: developer.nextbigsound.com\n    https: false\n    https_status: connection-refused\n\
  domains:\n  - domain: nextbigsound.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all\"\n    dmarc: true\n    dmarc_policy: reject\n    mx: [mx0a-0051e301.pphosted.com, mx0b-0051e301.pphosted.com]\n    nameservers: [ns2.pandora.com, ns4.pandora.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-big-sound/refs/heads/main/security/next-big-sound-domain-security.yml
summary_line: DMARC
tags:
- Company
- Music
- Analytics
- Data
- Metrics
- Social Media
- Media
- Acquired
---
