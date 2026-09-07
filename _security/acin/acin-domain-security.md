---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acin.com
  spf: true
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com; account=37519e363bd0f3f470682383a25b2daa13232906ff77b9eb03d1269486782a2a"
  - 0 issue "digicert.com; account=4735470c395ee719a2a0c2a15a49193ff5add1d47d164d31d186797e73892a18"
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 issue "microsoft.com"
  - 0 issuewild "microsoft.com"
  dmarc: false
  dnssec: false
  domain: azureedge.net
  spf: false
hosts:
- cert_expires: Nov 12 13:07:04 2026 GMT
  host: www.acin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 04:41:19 2027 GMT
  host: acin-documentation-prd01.azureedge.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 08:19:13 2026 GMT
  host: apim-prod.acin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Acin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acin
provider_slug: acin
slug: acin-domain-security
source_filename: acin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 13:07:04 2026 GMT\n  hsts: false\n- host: acin-documentation-prd01.azureedge.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 04:41:19 2027 GMT\n  hsts: false\n- host: apim-prod.acin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 08:19:13 2026 GMT\n  hsts: null\ndomains:\n- domain: acin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: azureedge.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com; account=37519e363bd0f3f470682383a25b2daa13232906ff77b9eb03d1269486782a2a\"\n  - 0 issue \"digicert.com; account=4735470c395ee719a2a0c2a15a49193ff5add1d47d164d31d186797e73892a18\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 issue \"microsoft.com\"\n \
  \ - 0 issuewild \"microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acin/refs/heads/main/security/acin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Operational Risk
- Risk Management
- Non-Financial Risk
- Financial Services
- Banking
- Compliance
- Regulatory Technology
- Benchmarking
- Data Standards
---
