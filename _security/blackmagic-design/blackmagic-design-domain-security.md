---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blackmagicdesign.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: blackmagicdesign.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blackmagic Design Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DaVinci Resolve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DaVinci Resolve
provider_slug: blackmagic-design
slug: blackmagic-design-domain-security
source_filename: blackmagic-design-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackmagicdesign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: blackmagicdesign.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/blackmagic-design/security/blackmagic-design-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- Broadcast
- Cinema
- Software
- Hardware
- Company
---
