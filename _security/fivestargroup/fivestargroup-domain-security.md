---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fivestargroup.in
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: fivestargroup.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fivestargroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fivestargroup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fivestargroup
provider_slug: fivestargroup
slug: fivestargroup-domain-security
source_filename: fivestargroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fivestargroup.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fivestargroup.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fivestargroup/refs/heads/main/security/fivestargroup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- NBFC
- Lending
- Loans
- Mortgage
- Fintech
- India
- Investor Relations
---
