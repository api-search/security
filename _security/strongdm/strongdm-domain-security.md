---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: strongdm.com
  spf: true
hosts:
- cert_expires: Sep 20 04:13:52 2026 GMT
  host: www.strongdm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:31:43 2026 GMT
  host: docs.strongdm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: app.strongdm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strongdm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StrongDM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StrongDM
provider_slug: strongdm
slug: strongdm-domain-security
source_filename: strongdm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.strongdm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.strongdm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:31:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.strongdm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: strongdm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strongdm/refs/heads/main/security/strongdm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Privileged Access Management
- Zero Trust
- Access Management
- Identity
- Infrastructure
- Audit
- Compliance
- DevOps
---
