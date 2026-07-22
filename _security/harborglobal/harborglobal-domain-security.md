---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: harborglobal.com
  spf: true
hosts:
- cert_expires: Aug 29 01:39:30 2026 GMT
  host: harborglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harborglobal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harbor Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Harbor Global
provider_slug: harborglobal
slug: harborglobal-domain-security
source_filename: harborglobal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: harborglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:39:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: harborglobal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harborglobal/refs/heads/main/security/harborglobal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Legal Technology
- Legal Operations
- Consulting
- Professional Services
- Legal
- Managed Services
- Vendor Governance
- Artificial Intelligence
---
