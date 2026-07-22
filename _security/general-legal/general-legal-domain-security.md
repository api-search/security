---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: general.legal
  spf: true
hosts:
- cert_expires: Sep  6 01:25:34 2026 GMT
  host: general.legal
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: General Legal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Legal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: General Legal
provider_slug: general-legal
slug: general-legal-domain-security
source_filename: general-legal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: general.legal\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:25:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: general.legal\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-legal/refs/heads/main/security/general-legal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Legal
- Law Firm
- Legal Tech
- Contracts
- Contract Review
- Compliance
- Artificial Intelligence
- Startups
- Y Combinator
---
