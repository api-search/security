---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: domcop.com
  spf: false
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.domcop.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Open Page Rank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Page Rank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Page Rank
provider_slug: open-page-rank
slug: open-page-rank-domain-security
source_filename: open-page-rank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.domcop.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: domcop.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-page-rank/refs/heads/main/security/open-page-rank-domain-security.yml
summary_line: TLSv1.2
tags:
- Development
- Public APIs
---
