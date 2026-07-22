---
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: privado.ai
  spf: true
hosts:
- cert_expires: Sep 10 05:27:53 2026 GMT
  host: www.privado.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Privado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Privado, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Privado
provider_slug: privado
slug: privado-domain-security
source_filename: privado-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.privado.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:27:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: privado.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/privado/refs/heads/main/security/privado-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Devops
- Privacy
- Data Privacy
- Security
- DevSecOps
- Code Scanning
- Static Analysis
- Compliance
- Governance
- Privacy Engineering
---
