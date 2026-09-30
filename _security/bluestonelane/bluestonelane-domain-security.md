---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bluestonelane.com
  spf: true
hosts:
- cert_expires: Dec 25 18:16:30 2026 GMT
  host: bluestonelane.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bluestonelane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluestonelane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bluestonelane
provider_slug: bluestonelane
slug: bluestonelane-domain-security
source_filename: bluestonelane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluestonelane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 18:16:30 2026 GMT\n  hsts: false\ndomains:\n- domain: bluestonelane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluestonelane/refs/heads/main/security/bluestonelane-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Coffee
- Retail
- Subscription
- Sustainability
---
