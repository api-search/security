---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hiscoxgroup.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hiscox.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hiscox.co.uk
  note: The UK domain enforces DMARC p=reject while the US/global hiscox.com domain is still at p=none (monitor only), and the group corporate domain hiscoxgroup.com publishes neither SPF nor DMARC.
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.hiscoxgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:16:49 2026 GMT
  host: developer.hiscox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.hiscox.com
  hsts: true
  hsts_max_age: 86400
  https: true
  note: Serves an Apigee proxy fault on every unauthenticated path; no routable public proxy. HSTS max-age of 86400 is well below the 31536000 used on the marketing hosts.
  role: API gateway (Apigee)
  tls_max_negotiated: TLSv1.2
  tls_version: TLSv1.2
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.hiscox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: US retail website
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.hiscox.co.uk
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: UK retail website
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hiscox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hiscox, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Hiscox
provider_slug: hiscox
slug: hiscox-domain-security
source_filename: hiscox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The gateway host api.hiscox.com and the two retail websites were probed by hand\n  in the same round because they are not carried as baseURLs in apis.yml (Hiscox\n  documents no public base URL). The API gateway is the only Hiscox host that\n  caps at TLS 1.2, which corroborates the developer FAQ statement that TLS 1.2 is\n  the only supported version for SDBX and Production.\nhosts:\n- host: www.hiscoxgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hiscox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:16:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.hiscox.com\n  role: API gateway (Apigee)\n  https: true\n  tls_version: TLSv1.2\n  tls_max_negotiated: TLSv1.2\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age:\
  \ 86400\n  note: >-\n    Serves an Apigee proxy fault on every unauthenticated path; no routable\n    public proxy. HSTS max-age of 86400 is well below the 31536000 used on the\n    marketing hosts.\n- host: www.hiscox.com\n  role: US retail website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.hiscox.co.uk\n  role: UK retail website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: hiscoxgroup.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: hiscox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hiscox.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: >-\n    The UK domain enforces DMARC p=reject while the US/global hiscox.com domain\n    is still at p=none (monitor\
  \ only), and the group corporate domain\n    hiscoxgroup.com publishes neither SPF nor DMARC.\nsecurity_txt:\n  published: false\n  probed:\n  - https://developer.hiscox.com/.well-known/security.txt\n  - https://www.hiscox.com/.well-known/security.txt\n  - https://www.hiscox.co.uk/.well-known/security.txt\n  - https://www.hiscoxgroup.com/.well-known/security.txt\n  - https://api.hiscox.com/.well-known/security.txt\n  result: all 404\nvulnerability_disclosure:\n  published: false\n  probed:\n  - https://hackerone.com/hiscox\n  - https://bugcrowd.com/hiscox\n  - https://www.hiscoxgroup.com/responsible-disclosure\n  - https://www.hiscoxgroup.com/security\n  - https://www.hiscoxgroup.com/vulnerability-disclosure\n  result: >-\n    All 404 (the www.hiscox.com equivalents return 403 to non-browser clients, so\n    they are inconclusive rather than confirmed absent). No coordinated\n    vulnerability disclosure programme, bug bounty or security contact could be\n    found for a company that itself\
  \ sells cyber insurance and publishes an annual\n    Cyber Readiness Report.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiscox/refs/heads/main/security/hiscox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Specialty Insurance
- Cyber Insurance
- Underwriting
- Reinsurance
- Lloyd's of London
- Small Business Insurance
- Quote
- ACORD
- Carrier
- Cargo
- Marine
- Payments
- API Gateway
---
