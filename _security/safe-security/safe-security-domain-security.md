---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: safe.security
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: safeone.ai
  spf: true
hosts:
- cert_expires: Nov  9 19:05:30 2026 GMT
  host: safe.security
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 02:52:43 2026 GMT
  host: docs.safe.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: us.safeone.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Safe Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAFE Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SAFE Security
provider_slug: safe-security
slug: safe-security-domain-security
source_filename: safe-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safe.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 19:05:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.safe.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 02:52:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.safeone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: safe.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: safeone.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safe-security/refs/heads/main/security/safe-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Cyber Risk Quantification
- Third-Party Risk Management
- Continuous Threat Exposure Management
- AI Security Posture Management
- Risk Management
- Governance Risk and Compliance
- FAIR
- Vulnerability Management
---
