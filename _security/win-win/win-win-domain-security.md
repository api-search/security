---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trywinwin.com
  spf: false
hosts:
- cert_expires: Aug 22 11:49:17 2026 GMT
  host: trywinwin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Win Win Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Win-Win, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Win-Win
provider_slug: win-win
slug: win-win-domain-security
source_filename: win-win-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trywinwin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:49:17 2026 GMT\n  hsts: false\ndomains:\n- domain: trywinwin.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/win-win/refs/heads/main/security/win-win-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fundraising
- Nonprofit
- Charity
- Donations
- Gaming
- Social Impact
---
