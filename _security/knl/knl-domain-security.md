---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knl.fi
  spf: true
hosts:
- cert_expires: Oct 11 06:11:01 2026 GMT
  host: knl.fi
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KNL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KNL
provider_slug: knl
slug: knl-domain-security
source_filename: knl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knl.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 06:11:01 2026 GMT\n  hsts: false\ndomains:\n- domain: knl.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knl/refs/heads/main/security/knl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defence
- Radio Communications
- Software Defined Radio
- Tactical Communications
- Critical Communications
- HF
- Networking
- Finland
- Hardware
---
