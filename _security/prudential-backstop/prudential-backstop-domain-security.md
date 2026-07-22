---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "globalsign.com"
  - 0 issuevmc "digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prudential.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.prudential.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prudential Backstop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prudential Backstop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prudential Backstop
provider_slug: prudential-backstop
slug: prudential-backstop-domain-security
source_filename: prudential-backstop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prudential.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: prudential.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuevmc \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prudential-backstop/refs/heads/main/security/prudential-backstop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- 401k
- Backstop
- Financial Services
- Insurance
- Investments
- Pension
- Retirement
---
