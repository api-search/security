---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "amazonaws.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: diligent.com
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: highbond.com
  spf: true
hosts:
- cert_expires: Oct  5 21:13:49 2026 GMT
  host: www.diligent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: developer.diligent.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: apis-us.highbond.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Diligent Boards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diligent, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Diligent
provider_slug: diligent-boards
slug: diligent-boards-domain-security
source_filename: diligent-boards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diligent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.diligent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: apis-us.highbond.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: diligent.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: highbond.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diligent-boards/refs/heads/main/security/diligent-boards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Governance
- Risk
- Compliance
- GRC
- Board Management
- Audit
- Entity Management
- ESG
- Enterprise
---
