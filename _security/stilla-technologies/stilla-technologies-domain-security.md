---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stillatechnologies.com
  spf: false
hosts:
- cert_expires: Aug 28 17:50:11 2026 GMT
  host: www.stillatechnologies.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stilla Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stilla Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Stilla Technologies
provider_slug: stilla-technologies
slug: stilla-technologies-domain-security
source_filename: stilla-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stillatechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 17:50:11 2026 GMT\n  hsts: null\ndomains:\n- domain: stillatechnologies.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stilla-technologies/refs/heads/main/security/stilla-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Life Sciences
- Diagnostics
- Digital PCR
- Genomics
- Biotechnology
- Laboratory Instruments
---
