---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: betr.app
  spf: true
hosts:
- cert_expires: Oct 24 20:11:06 2026 GMT
  host: www.betr.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 00:18:12 2026 GMT
  host: api.betr.app
  hsts: false
  https: true
  note: Private API backend; anonymous requests return HTTP 500 or 403.
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:41:35 2026 GMT
  host: picks.betr.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 06:35:46 2026 GMT
  host: help.betr.app
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_preload: true
  https: true
  note: Intercom-hosted help center; the HSTS posture is the vendor's, not a Betr origin.
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: stage1-backoffice-api-docs.betr.app
  hsts: false
  https: true
  note: Staging back-office API docs host (AWS ELB, us-east-1); HTTP 403 on every path.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Betr, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Betr
provider_slug: betr
slug: betr-domain-security
source_filename: betr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + contract-discovery hosts\nhosts:\n- host: www.betr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 20:11:06 2026 GMT\n  hsts: false\n- host: api.betr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:18:12 2026 GMT\n  hsts: false\n  note: Private API backend; anonymous requests return HTTP 500 or 403.\n- host: picks.betr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:41:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.betr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 06:35:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Intercom-hosted help center; the HSTS posture is the vendor's, not a Betr origin.\n- host: stage1-backoffice-api-docs.betr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n\
  \  hsts: false\n  note: Staging back-office API docs host (AWS ELB, us-east-1); HTTP 403 on every path.\ndomains:\n- domain: betr.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nfindings:\n- No CAA records are published on betr.app.\n- No HSTS on the primary marketing host (www.betr.app) or on the API host (api.betr.app);\n  HSTS is present only on picks.betr.app and the vendor-hosted help center.\n- DNSSEC is enabled on betr.app; the DMARC policy is quarantine, not reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betr/refs/heads/main/security/betr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Gaming
- Sports Betting
- Daily Fantasy Sports
- Sports
- Media
- Entertainment
- Mobile Apps
- Consumer
- Responsible Gaming
---
