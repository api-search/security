---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mellowmountainradio.com
  spf: true
hosts:
- cert_expires: Jan 27 02:13:54 2027 GMT
  host: mellowmountainradio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mellow Mountain Radio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mellow Mountain Radio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mellow Mountain Radio
provider_slug: mellowmountainradio-com
slug: mellowmountainradio-com-domain-security
source_filename: mellowmountainradio-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mellowmountainradio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 02:13:54 2027 GMT\n  hsts: false\ndomains:\n- domain: mellowmountainradio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mellowmountainradio-com/security/mellowmountainradio-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Radio
- Media
- Community
- Arizona
- Streaming
---
