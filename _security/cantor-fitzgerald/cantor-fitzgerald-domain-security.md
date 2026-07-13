---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cantor.com
  spf: true
- caa:
  - 0 issue "entrust.net"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 iodef "mailto:CAIssues@sec.gov"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sec.gov
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.cantor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.sec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 12:38:45 2026 GMT
  host: www.bgcgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cantor Fitzgerald Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cantor Fitzgerald, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cantor Fitzgerald
provider_slug: cantor-fitzgerald
slug: cantor-fitzgerald-domain-security
source_filename: cantor-fitzgerald-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cantor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\n- host: www.sec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: www.bgcgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:38:45 2026 GMT\n  hsts: false\ndomains:\n- domain: cantor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sec.gov\n  dnssec: true\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:CAIssues@sec.gov\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cantor-fitzgerald/refs/heads/main/security/cantor-fitzgerald-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial Services
- Investment Banking
- Prime Brokerage
- Fixed Income
- Equities
- Real Estate Finance
- Market Data
- SPAC
---
