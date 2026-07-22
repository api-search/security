---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reetian.com
  spf: false
hosts:
- cert_expires: Aug 23 07:08:14 2026 GMT
  host: reetian.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reetian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for reetian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: reetian
provider_slug: reetian
slug: reetian-domain-security
source_filename: reetian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reetian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 07:08:14 2026 GMT\n  hsts: false\ndomains:\n- domain: reetian.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reetian/refs/heads/main/security/reetian-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- China
- Digital Intelligence
- Data
- Analytics
- Enterprise
---
