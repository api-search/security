---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: horizonmedia.com
  spf: true
hosts:
- cert_expires: Sep  3 14:12:09 2026 GMT
  host: www.horizonmedia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Horizon Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Horizon Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Horizon Media
provider_slug: horizon-media
slug: horizon-media-domain-security
source_filename: horizon-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.horizonmedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 14:12:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: horizonmedia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon-media/refs/heads/main/security/horizon-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Advertising
- Media Agency
- Media Planning
- Media Buying
- Programmatic
- Retail Media
- Sports Marketing
- Social Media
- Influencer Marketing
- Cultural Intelligence
- Data Platform
- AI Platform
- MarTech
- AdTech
- Independent Agency
---
