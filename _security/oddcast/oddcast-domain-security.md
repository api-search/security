---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oddcast.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vocalware.com
  spf: true
hosts:
- cert_expires: Sep  7 23:59:59 2026 GMT
  host: oddcast.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.vocalware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:59:59 2026 GMT
  host: www.sitepal.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Oddcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oddcast, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Oddcast
provider_slug: oddcast
slug: oddcast-domain-security
source_filename: oddcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oddcast.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  7 23:59:59 2026 GMT\n  hsts: false\n- host: www.vocalware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n- host: www.sitepal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: oddcast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vocalware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oddcast/refs/heads/main/security/oddcast-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Text-to-Speech
- Speech Synthesis
- Avatars
- Voice
- Media
- Creative Technology
- Education
- Developers
---
