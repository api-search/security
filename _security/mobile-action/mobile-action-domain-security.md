---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mobileaction.co
  spf: true
hosts:
- cert_expires: Sep 20 09:32:07 2026 GMT
  host: mobileaction.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 09:32:07 2026 GMT
  host: docs.mobileaction.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 09:32:07 2026 GMT
  host: api.mobileaction.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mobile Action Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mobile Action, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mobile Action
provider_slug: mobile-action
slug: mobile-action-domain-security
source_filename: mobile-action-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mobileaction.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:32:07 2026 GMT\n  hsts: false\n- host: docs.mobileaction.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:32:07 2026 GMT\n  hsts: false\n- host: api.mobileaction.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 09:32:07 2026 GMT\n  hsts: null\ndomains:\n- domain: mobileaction.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobile-action/refs/heads/main/security/mobile-action-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- App Store Optimization
- ASO
- Mobile Marketing
- Apple Search Ads
- App Intelligence
- Ad Intelligence
- Market Intelligence
- Analytics
- MCP
- Agent Tools
- App Store Intelligence
- Mobile Measurement
---
