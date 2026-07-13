---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bombora.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  spf: true
hosts:
- cert_expires: Sep 28 18:04:07 2026 GMT
  host: bombora.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:47:56 2026 GMT
  host: developer.bombora.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: bombora-partners.atlassian.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bombora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bombora, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bombora
provider_slug: bombora
slug: bombora-domain-security
source_filename: bombora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bombora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:04:07 2026 GMT\n  hsts: false\n- host: developer.bombora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:47:56 2026 GMT\n  hsts: null\n- host: bombora-partners.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bombora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bombora/refs/heads/main/security/bombora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Intent Data
- B2B Intent
- Company Surge
- Account Based Marketing
- Sales Intelligence
- Marketing Intelligence
- Identity Resolution
- Audience Activation
- Data Cooperative
- Webhooks
- Reference Data
- Adtech
- Martech
- B2B
---
