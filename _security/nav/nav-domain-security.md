---
description: ''
domains:
- caa:
  - 0 iodef "mailto:eng-serv@nav.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nav.com
  spf: true
hosts:
- cert_expires: Nov  8 16:13:40 2026 GMT
  host: www.nav.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  8 16:13:40 2026 GMT
  host: api-docs.nav.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  8 16:13:40 2026 GMT
  host: api.nav.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nav Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nav, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nav
provider_slug: nav
slug: nav-domain-security
source_filename: nav-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nav.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 16:13:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api-docs.nav.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 16:13:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.nav.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 16:13:40 2026 GMT\n  hsts: null\ndomains:\n- domain: nav.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:eng-serv@nav.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nav/refs/heads/main/security/nav-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Business Credit
- Small Business
- Financial Services
- Embedded Finance
- Lending
- Credit Scores
- Credit Reporting
- Financing Marketplace
- Fintech
- Partner API
---
