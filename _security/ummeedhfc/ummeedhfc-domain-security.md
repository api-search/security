---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ummeedhfc.com
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: ummeedhfc.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ummeedhfc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ummeed Housing Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ummeed Housing Finance
provider_slug: ummeedhfc
slug: ummeedhfc-domain-security
source_filename: ummeedhfc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ummeedhfc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: ummeedhfc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ummeedhfc/refs/heads/main/security/ummeedhfc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Housing Finance
- Home Loans
- Lending
- Financial Services
- MSME
- India
---
