---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vrchat.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vrchat.cloud
  spf: false
hosts:
- cert_expires: Sep 30 19:25:54 2026 GMT
  host: hello.vrchat.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.vrchat.cloud
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 17:30:50 2026 GMT
  host: vcc.docs.vrchat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vrchat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VRChat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VRChat
provider_slug: vrchat
slug: vrchat-domain-security
source_filename: vrchat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hello.vrchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 19:25:54 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.vrchat.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: vcc.docs.vrchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 17:30:50 2026 GMT\n  hsts: false\ndomains:\n- domain: vrchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vrchat.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vrchat/refs/heads/main/security/vrchat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Virtual Reality
- Social Networks
- Gaming
- Metaverse
- Avatars
- Unity
- Creator Economy
- User Generated Content
- OSC
---
