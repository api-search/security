---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: mondoo.com
  spf: true
hosts:
- cert_expires: Oct 15 01:13:11 2026 GMT
  host: mondoo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 10:30:39 2026 GMT
  host: us.api.mondoo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mondoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mondoo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Mondoo
provider_slug: mondoo
slug: mondoo-domain-security
source_filename: mondoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mondoo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:13:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.api.mondoo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:30:39 2026 GMT\n  hsts: null\ndomains:\n- domain: mondoo.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mondoo/refs/heads/main/security/mondoo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Security
- Vulnerability Management
- Compliance
- Cloud Security
- Policy as Code
- DevSecOps
- GraphQL
- SAST
---
