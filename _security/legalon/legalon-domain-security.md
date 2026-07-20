---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: legalontech.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: legalontech.jp
  spf: true
hosts:
- cert_expires: Oct  1 03:11:15 2026 GMT
  host: www.legalontech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 10:47:16 2026 GMT
  host: legalontech.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 06:01:53 2026 GMT
  host: api.legalontech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Legalon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LegalOn, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: LegalOn
provider_slug: legalon
slug: legalon-domain-security
source_filename: legalon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.legalontech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:11:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: legalontech.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:47:16 2026 GMT\n  hsts: false\n- host: api.legalontech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:01:53 2026 GMT\n  hsts: null\ndomains:\n- domain: legalontech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: legalontech.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legalon/refs/heads/main/security/legalon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Technology
- Legal
- Legal Technology
- Contracts
- Contract Management
- Contract Lifecycle Management
- Artificial Intelligence
- Document Management
- Compliance
- Governance
- SaaS
- Japan
---
