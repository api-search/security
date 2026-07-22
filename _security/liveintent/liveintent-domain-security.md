---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: liveintent.com
  spf: true
hosts:
- cert_expires: Sep 16 14:17:34 2026 GMT
  host: www.liveintent.com
  hsts: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liveintent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveIntent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LiveIntent
provider_slug: liveintent
slug: liveintent-domain-security
source_filename: liveintent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liveintent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 14:17:34 2026 GMT\n  hsts: true\ndomains:\n- domain: liveintent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveintent/refs/heads/main/security/liveintent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Identity
- Email Marketing
- Audience
- Publishers
- Marketers
- Data
---
