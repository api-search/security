---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: seqholdings.com
  spf: false
hosts:
- cert_expires: Sep 23 15:31:27 2026 GMT
  host: seqholdings.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequence Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequence Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Sequence Holdings
provider_slug: sequence-holdings
slug: sequence-holdings-domain-security
source_filename: sequence-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seqholdings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:31:27 2026 GMT\n  hsts: false\ndomains:\n- domain: seqholdings.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequence-holdings/refs/heads/main/security/sequence-holdings-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Holding Company
- Artificial Intelligence
- Business Acquisition
- Technology
- Investment
---
