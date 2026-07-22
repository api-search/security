---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: mailto:dmarc-reports@linxsecurity.io
  dnssec: true
  domain: linx.security
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: mailto:dmarc-reports@linxsecurity.io
  dnssec: false
  domain: linxsecurity.io
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:145005636.spf03.hubspotemail.net -all
hosts:
- cert_expires: Oct 11 03:11:14 2026 GMT
  host: www.linx.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 11:22:36 2026 GMT
  host: trust.linx.security
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: app.linxsecurity.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 02:35:50 2026 GMT
  host: docs.linxsecurity.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 22:00:07 2026 GMT
  host: status.linxsecurity.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63113904
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linx Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linx Security, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Linx Security
provider_slug: linx-security
slug: linx-security-domain-security
source_filename: linx-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the linxsecurity.io product hosts\nnotes: >-\n  Linx operates two registrable domains: linx.security (marketing site, Webflow\n  behind Cloudflare) and linxsecurity.io (product app, docs/login, status page).\n  Both enforce DMARC p=reject. linx.security has DNSSEC enabled (Cloudflare\n  universal signing) but publishes no SPF on the apex and no CAA; linxsecurity.io\n  publishes SPF but no DNSSEC and no CAA. Absence of a record is recorded data,\n  not an error.\nhosts:\n- host: www.linx.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 03:11:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: trust.linx.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:22:36 2026 GMT\n  hsts: false\n- host: app.linxsecurity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: false\n- host: docs.linxsecurity.io\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:35:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: status.linxsecurity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:00:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63113904\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: linx.security\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: mailto:dmarc-reports@linxsecurity.io\n- domain: linxsecurity.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:amazonses.com include:145005636.spf03.hubspotemail.net\n    -all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: mailto:dmarc-reports@linxsecurity.io\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linx-security/refs/heads/main/security/linx-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Identity
- Identity Governance
- Access Management
- Identity Security
- Non-Human Identity
- Agentic AI
- MCP
- IGA
---
