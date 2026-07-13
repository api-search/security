---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ketch.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ketchapi.com
  spf: false
hosts:
- cert_expires: Aug 28 08:13:20 2026 GMT
  host: www.ketch.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 12:20:18 2026 GMT
  host: docs.ketch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 06:13:34 2026 GMT
  host: global.ketchapi.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ketch Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ketch, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ketch
provider_slug: ketch-com
slug: ketch-com-domain-security
source_filename: ketch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ketch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:13:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.ketch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:20:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: global.ketchapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 06:13:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: ketch.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ketchapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ketch-com/refs/heads/main/security/ketch-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Privacy
- Consent
- Data Permissioning
- DSR
- Data Mapping
- AI Governance
- Preference Management
- Risk
- GDPR
- CCPA
- CPRA
- Switchbit
---
