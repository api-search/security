---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jitsi.org
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:dns-management@8x8.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 8x8.com
  spf: true
hosts:
- cert_expires: Oct  3 03:42:28 2026 GMT
  host: jitsi.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 06:24:19 2026 GMT
  host: developer.8x8.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.jaas.8x8.vc
  https: false
kind: domain-security
layout: security
method: probed
name: Jitsi Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jitsi, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jitsi
provider_slug: jitsi
slug: jitsi-org-domain-security
source_filename: jitsi-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jitsi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:42:28 2026 GMT\n  hsts: false\n- host: developer.8x8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:24:19 2026 GMT\n  hsts: false\n- host: api.jaas.8x8.vc\n  https: false\ndomains:\n- domain: jitsi.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: 8x8.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:dns-management@8x8.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jitsi/refs/heads/main/security/jitsi-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video Conferencing
- WebRTC
- Real-Time Communication
- Open Source
- Voice
- Video
- SIP
- Streaming
- Recording
- Self-Hosted
---
