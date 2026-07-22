---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: comstruct.com
  spf: true
hosts:
- cert_expires: Oct  7 17:36:42 2026 GMT
  host: www.comstruct.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comstruct Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comstruct, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Comstruct
provider_slug: comstruct
slug: comstruct-domain-security
source_filename: comstruct-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comstruct.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:36:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: comstruct.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comstruct/refs/heads/main/security/comstruct-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Construction
- Construction Technology
- Procurement
- Supply Chain
- Invoice Automation
- Fintech
- Artificial Intelligence
- Germany
---
