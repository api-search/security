---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wellframe.com
  spf: true
hosts:
- cert_expires: Oct  5 19:18:19 2026 GMT
  host: www.wellframe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellframe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wellframe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wellframe
provider_slug: wellframe
slug: wellframe-domain-security
source_filename: wellframe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wellframe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:18:19 2026 GMT\n  hsts: false\ndomains:\n- domain: wellframe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellframe/refs/heads/main/security/wellframe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Care Management
- Member Engagement
- Health Plans
- Payer
---
