---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: whipmedia.com
  spf: true
hosts:
- cert_expires: Sep 21 07:38:32 2026 GMT
  host: www.whipmedia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whip Media Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whip Media Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Whip Media Group
provider_slug: whip-media-group
slug: whip-media-group-domain-security
source_filename: whip-media-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.whipmedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:38:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whipmedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whip-media-group/refs/heads/main/security/whip-media-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Entertainment
- Content Licensing
- SaaS
- Metadata
- Royalties
- Rights Management
---
