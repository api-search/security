---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: tlapl.us
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inria.fr
  spf: true
hosts:
- cert_expires: Sep 17 12:47:48 2026 GMT
  host: foundation.tlapl.us
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: tla.msr-inria.inria.fr
  https: false
- cert_expires: Sep  6 13:38:08 2026 GMT
  host: marketplace.visualstudio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tla Plus Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TLA Plus Foundation, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TLA Plus Foundation
provider_slug: tla-plus-foundation
slug: tla-plus-foundation-domain-security
source_filename: tla-plus-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foundation.tlapl.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 12:47:48 2026 GMT\n  hsts: false\n- host: tla.msr-inria.inria.fr\n  https: false\n- host: marketplace.visualstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:38:08 2026 GMT\n  hsts: null\ndomains:\n- domain: tlapl.us\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n- domain: inria.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tla-plus-foundation/refs/heads/main/security/tla-plus-foundation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Formal Methods
- Linux Foundation
- Specifications
- Verification
- Distributed Systems
- Concurrency
---
