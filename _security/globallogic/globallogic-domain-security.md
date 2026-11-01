---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globallogic.com
  spf: true
hosts:
- cert_expires: Nov 10 12:45:20 2026 GMT
  host: www.globallogic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Globallogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GlobalLogic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GlobalLogic
provider_slug: globallogic
slug: globallogic-domain-security
source_filename: globallogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globallogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 12:45:20 2026 GMT\n  hsts: null\ndomains:\n- domain: globallogic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/globallogic/security/globallogic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Digital Engineering
- Product Strategy
- Software Product Engineering
- Intelligence Engineering
- Technology Modernization
- Embedded Engineering
---
