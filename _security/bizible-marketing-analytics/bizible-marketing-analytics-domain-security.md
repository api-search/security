---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bizible.com
  spf: true
hosts:
- cert_expires: Oct  2 19:34:56 2026 GMT
  host: bizible.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bizible Marketing Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bizible Marketing Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bizible Marketing Analytics
provider_slug: bizible-marketing-analytics
slug: bizible-marketing-analytics-domain-security
source_filename: bizible-marketing-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bizible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:34:56 2026 GMT\n  hsts: null\ndomains:\n- domain: bizible.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bizible-marketing-analytics/refs/heads/main/security/bizible-marketing-analytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- Analytics
- Marketing Attribution
- Revenue Analytics
- B2B
- Adobe
- Marketo
---
