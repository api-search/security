---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oasislabs.com
  spf: true
hosts:
- cert_expires: Sep 13 00:14:16 2026 GMT
  host: www.oasislabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 11:32:43 2026 GMT
  host: docs.oasislabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:33:22 2026 GMT
  host: api.oasislabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oasis Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oasis Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oasis Labs
provider_slug: oasis-labs
slug: oasis-labs-domain-security
source_filename: oasis-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oasislabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:14:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.oasislabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:32:43 2026 GMT\n  hsts: false\n- host: api.oasislabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:33:22 2026 GMT\n  hsts: null\ndomains:\n- domain: oasislabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oasis-labs/refs/heads/main/security/oasis-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Privacy
- Data Governance
- Confidential Computing
- Blockchain
- Differential Privacy
- Machine Learning
- Developer Platform
- Web3
---
