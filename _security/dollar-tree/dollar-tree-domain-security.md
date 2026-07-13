---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dollartree.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.dollartree.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: cvp.dollartree.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dollar Tree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dollar Tree, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dollar Tree
provider_slug: dollar-tree
slug: dollar-tree-domain-security
source_filename: dollar-tree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dollartree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\n- host: cvp.dollartree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dollartree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dollar-tree/refs/heads/main/security/dollar-tree-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Retail
- Discount Retail
- EDI
- Vendor Management
- Fortune 500
---
