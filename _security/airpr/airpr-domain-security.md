---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onclusive.com
  spf: true
hosts:
- cert_expires: Oct  1 21:56:45 2026 GMT
  host: onclusive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airpr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirPR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AirPR
provider_slug: airpr
slug: airpr-domain-security
source_filename: airpr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onclusive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:56:45 2026 GMT\n  hsts: false\ndomains:\n- domain: onclusive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airpr/refs/heads/main/security/airpr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Public Relations
- Media Intelligence
- Media Monitoring
- Analytics
- Communications
- Marketing
- PR Measurement
- Onclusive
---
