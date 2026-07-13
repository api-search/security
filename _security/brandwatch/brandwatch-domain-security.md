---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brandwatch.com
  spf: true
hosts:
- cert_expires: Aug 13 08:15:00 2026 GMT
  host: www.brandwatch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brandwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandwatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brandwatch
provider_slug: brandwatch
slug: brandwatch-domain-security
source_filename: brandwatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brandwatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 08:15:00 2026 GMT\n  hsts: false\ndomains:\n- domain: brandwatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/security/brandwatch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Social Media
- Social Media Monitoring
- Consumer Intelligence
- Brand Management
- Sentiment Analysis
---
