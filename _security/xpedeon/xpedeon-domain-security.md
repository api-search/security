---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xpedeon.com
  spf: false
hosts:
- cert_expires: Sep 29 04:43:45 2026 GMT
  host: xpedeon.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Xpedeon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xpedeon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Xpedeon
provider_slug: xpedeon
slug: xpedeon-domain-security
source_filename: xpedeon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xpedeon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 04:43:45 2026 GMT\n  hsts: false\ndomains:\n- domain: xpedeon.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xpedeon/refs/heads/main/security/xpedeon-domain-security.yml
summary_line: TLSv1.2
tags:
- Construction
- ERP
- Job Costing
- Procurement
- Contract Management
- Subcontractor Management
- Construction Accounting
---
