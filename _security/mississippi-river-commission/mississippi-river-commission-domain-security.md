---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: army.mil
  spf: true
hosts:
- cert_expires: Aug  3 14:09:16 2026 GMT
  host: www.mvd.usace.army.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mississippi River Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mississippi River Commission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mississippi River Commission
provider_slug: mississippi-river-commission
slug: mississippi-river-commission-domain-security
source_filename: mississippi-river-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mvd.usace.army.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 14:09:16 2026 GMT\n  hsts: null\ndomains:\n- domain: army.mil\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mississippi-river-commission/refs/heads/main/security/mississippi-river-commission-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Flood Control
- Mississippi River
- Navigation
- River Management
- US Army Corps of Engineers
- Water Resources
---
