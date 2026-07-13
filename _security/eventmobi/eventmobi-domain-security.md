---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eventmobi.com
  spf: true
hosts:
- cert_expires: Sep 27 14:26:53 2026 GMT
  host: www.eventmobi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: developers.eventmobi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: uapi.eventmobi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eventmobi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EventMobi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EventMobi
provider_slug: eventmobi
slug: eventmobi-domain-security
source_filename: eventmobi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eventmobi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:26:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.eventmobi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\n- host: uapi.eventmobi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: eventmobi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventmobi/refs/heads/main/security/eventmobi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Events
- Event Management
- Event Apps
- Attendees
- Sessions
- Registration
---
