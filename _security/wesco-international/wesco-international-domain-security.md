---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wesco.com
  spf: true
hosts:
- cert_expires: Sep  9 18:26:28 2026 GMT
  host: www.wesco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 14:20:35 2026 GMT
  host: buy.wesco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wesco International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WESCO International, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WESCO International
provider_slug: wesco-international
slug: wesco-international-domain-security
source_filename: wesco-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wesco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:26:28 2026 GMT\n  hsts: null\n- host: buy.wesco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 14:20:35 2026 GMT\n  hsts: null\ndomains:\n- domain: wesco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wesco-international/refs/heads/main/security/wesco-international-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Distribution
- Supply Chain
- Electrical
- Industrial
- Procurement
- B2B
- EDI
- Fortune 500
---
