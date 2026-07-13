---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pagecdn.com
  spf: true
hosts:
- cert_expires: Oct 10 06:22:12 2026 GMT
  host: pagecdn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pagecdn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PageCDN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PageCDN
provider_slug: pagecdn
slug: pagecdn-domain-security
source_filename: pagecdn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagecdn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:22:12 2026 GMT\n  hsts: false\ndomains:\n- domain: pagecdn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pagecdn/refs/heads/main/security/pagecdn-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---
