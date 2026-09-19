---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jssict.com
  spf: true
hosts:
- cert_expires: Feb 19 07:05:28 2027 GMT
  host: www.jssict.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aichengtechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aicheng Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aicheng Technology
provider_slug: aichengtechnology
slug: aichengtechnology-domain-security
source_filename: aichengtechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jssict.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 19 07:05:28 2027 GMT\n  hsts: false\ndomains:\n- domain: jssict.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aichengtechnology/refs/heads/main/security/aichengtechnology-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Semiconductors
- Advanced Materials
- Ceramics
- Manufacturing
- Electronic Components
- Hardware
---
