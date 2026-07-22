---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: native.security
  spf: true
hosts:
- cert_expires: Oct 12 12:36:17 2026 GMT
  host: native.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Native Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Native Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Native Security
provider_slug: native-security
slug: native-security-domain-security
source_filename: native-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: native.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 12:36:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: native.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/native-security/refs/heads/main/security/native-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Cloud Security
- Cloud
- Compliance
- Governance
- Multi-Cloud
- AI Security
---
