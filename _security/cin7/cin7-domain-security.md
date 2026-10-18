---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:securityteam@cin7.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cin7.com
  spf: true
hosts:
- cert_expires: Dec 16 19:47:47 2026 GMT
  host: www.cin7.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cin7 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cin7, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cin7
provider_slug: cin7
slug: cin7-domain-security
source_filename: cin7-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cin7.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 19:47:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cin7.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:securityteam@cin7.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cin7/refs/heads/main/security/cin7-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Inventory
- ERP
- Retail
- Integration
---
