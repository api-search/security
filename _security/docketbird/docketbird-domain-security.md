---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: docketbird.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: www.docketbird.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docketbird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocketBird, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DocketBird
provider_slug: docketbird
slug: docketbird-domain-security
source_filename: docketbird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docketbird.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: docketbird.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docketbird/refs/heads/main/security/docketbird-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Legal Tech
- CourtFiling
- Document-Management
- Automation
---
