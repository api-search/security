---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: silverpush.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chocolateplatform.com
  spf: true
hosts:
- cert_expires: Oct 12 09:50:07 2026 GMT
  host: silverpush.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 07:52:46 2026 GMT
  host: chocolateplatform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 08:30:18 2026 GMT
  host: docs.prebid.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silveredge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silveredge, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Silveredge
provider_slug: silveredge
slug: silveredge-domain-security
source_filename: silveredge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silverpush.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 09:50:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: chocolateplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:52:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.prebid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:30:18 2026 GMT\n  hsts: false\ndomains:\n- domain: silverpush.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: chocolateplatform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silveredge/refs/heads/main/security/silveredge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Contextual Intelligence
- Artificial Intelligence
- Video Advertising
- Marketing
- Programmatic Advertising
- OpenRTB
- Prebid
- Supply Side Platform
- CTV
- Mobile Advertising
- Brand Safety
---
