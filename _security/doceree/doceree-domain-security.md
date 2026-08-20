---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doceree.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: doceree.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: bidder.doceree.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: tracking.doceree.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Doceree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doceree, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Doceree
provider_slug: doceree
slug: doceree-domain-security
source_filename: doceree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doceree.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\n- host: bidder.doceree.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\n- host: tracking.doceree.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: doceree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doceree/refs/heads/main/security/doceree-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Advertising
- Healthcare
- Marketing
- AdTech
- Programmatic
- Header Bidding
- Life Sciences
- Pharmaceuticals
- Point of Care
- Identity Resolution
- Electronic Health Records
- Company
---
