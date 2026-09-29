---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
hosts:
- cert_expires: Dec 18 16:17:45 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bitgravity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitGravity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BitGravity
provider_slug: bitgravity
slug: bitgravity-domain-security
source_filename: bitgravity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 16:17:45 2026 GMT\n  hsts: null\ndomains:\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitgravity/refs/heads/main/security/bitgravity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Content Delivery Network
- Enterprise Software
- Cloud Networking
- Video Streaming
- Live Streaming
---
