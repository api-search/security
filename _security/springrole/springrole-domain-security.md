---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: springrole.com
  spf: true
hosts:
- cert_expires: Oct 15 14:46:33 2026 GMT
  host: springrole.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Springrole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpringRole, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SpringRole
provider_slug: springrole
slug: springrole-domain-security
source_filename: springrole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: springrole.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 14:46:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: springrole.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/springrole/refs/heads/main/security/springrole-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Blockchain
- Professional Reputation
- Attestation
- Web3
- Recruiting
- HR
---
