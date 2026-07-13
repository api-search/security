---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ropertech.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aderant.com
  spf: true
hosts:
- cert_expires: Sep 21 14:50:28 2026 GMT
  host: www.ropertech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 06:48:11 2026 GMT
  host: www.aderant.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 17:03:41 2026 GMT
  host: www.clinisys.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roper Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roper Technologies, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Roper Technologies
provider_slug: roper-technologies
slug: roper-technologies-domain-security
source_filename: roper-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ropertech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:50:28 2026 GMT\n  hsts: null\n- host: www.aderant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:48:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.clinisys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:03:41 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: ropertech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aderant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roper-technologies/refs/heads/main/security/roper-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- B2B Software
- Enterprise Software
- Fortune 500
- Healthcare IT
- Insurance Technology
- Legal Technology
- SaaS
- Vertical Software
---
