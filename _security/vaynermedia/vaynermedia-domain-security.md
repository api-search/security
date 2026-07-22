---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vaynermedia.com
  spf: true
hosts:
- cert_expires: Oct  3 02:49:40 2026 GMT
  host: vaynermedia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vaynermedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VaynerMedia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VaynerMedia
provider_slug: vaynermedia
slug: vaynermedia-domain-security
source_filename: vaynermedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vaynermedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:49:40 2026 GMT\n  hsts: false\ndomains:\n- domain: vaynermedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vaynermedia/refs/heads/main/security/vaynermedia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Agency
- Brand Strategy
- Content Production
- Creative
- Influencer Marketing
- Marketing
- Media Buying
- Social Media
---
