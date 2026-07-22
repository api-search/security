---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xsightlabs.com
  spf: true
hosts:
- cert_expires: Sep 11 05:58:11 2026 GMT
  host: xsightlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xsight Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xsight Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Xsight Labs
provider_slug: xsight-labs
slug: xsight-labs-domain-security
source_filename: xsight-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xsightlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:58:11 2026 GMT\n  hsts: null\ndomains:\n- domain: xsightlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xsight-labs/refs/heads/main/security/xsight-labs-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Semiconductors
- Networking
- Data Center
- Switch Silicon
- DPU
- AI Infrastructure
- SONiC
- Ethernet
- Hardware
---
