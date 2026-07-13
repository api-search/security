---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:domainmgr@capitalone.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: capitalone.com
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: developer.capitalone.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capital One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capital One, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Capital One
provider_slug: capital-one
slug: capital-one-domain-security
source_filename: capital-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.capitalone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: capitalone.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:domainmgr@capitalone.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capital-one/refs/heads/main/security/capital-one-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Auto Finance
- Authorizations
- Banking
- Credit Cards
- Credit Offers
- DevExchange
- Financial Services
- OAuth 2.0
- Payments
- Rewards
- Fortune 500
---
