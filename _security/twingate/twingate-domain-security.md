---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: twingate.com
  spf: true
hosts:
- cert_expires: Aug 18 18:40:45 2026 GMT
  host: www.twingate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twingate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twingate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Twingate
provider_slug: twingate
slug: twingate-domain-security
source_filename: twingate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twingate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 18:40:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: twingate.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twingate/refs/heads/main/security/twingate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Zero Trust
- ZTNA
- Network Access
- VPN Replacement
- Identity-Based Access
- Security
---
