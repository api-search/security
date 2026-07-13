---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sequoiacap.com
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crunchbase.com
  spf: true
hosts:
- cert_expires: Oct  5 12:35:24 2026 GMT
  host: www.sequoiacap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 12:58:43 2026 GMT
  host: data.crunchbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 23:43:35 2026 GMT
  host: pitchbook.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequoia Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequoia Capital, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sequoia Capital
provider_slug: sequoia-capital
slug: sequoia-capital-domain-security
source_filename: sequoia-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sequoiacap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:35:24 2026 GMT\n  hsts: false\n- host: data.crunchbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:58:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pitchbook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:43:35 2026 GMT\n  hsts: null\ndomains:\n- domain: sequoiacap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: crunchbase.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequoia-capital/refs/heads/main/security/sequoia-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Venture Capital
- Investment
- Startup Funding
- Private Equity
- Portfolio Management
---
