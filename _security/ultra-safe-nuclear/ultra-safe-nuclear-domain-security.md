---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; pct=100; rua=mailto:dmarc@usnc.com; ruf=mailto:dmarc@usnc.com; fo=1
  dnssec: false
  domain: usnc.com
  mx:
  - usnctech.mail.protection.office365.us
  nameservers:
  - ns27.domaincontrol.com
  - ns28.domaincontrol.com
  registrar: GoDaddy Online Services Cayman Islands Ltd.
  registry_expiry: '2027-03-12'
  spf: true
  spf_record: v=spf1 include:spf.protection.office365.us -all
  web_presence: false
- caa: []
  created: '2022-03-30'
  dmarc: false
  dnssec: true
  domain: ultrasafenuclear.com
  mx: []
  nameservers:
  - ns-cloud-b1.googledomains.com
  - ns-cloud-b2.googledomains.com
  - ns-cloud-b3.googledomains.com
  - ns-cloud-b4.googledomains.com
  ownership: unverified
  registrar: null
  registry_expiry: '2032-03-30'
  spf: false
  web_presence: placeholder
hosts:
- host: usnc.com
  hsts: null
  https: false
  reachable: false
  reason: NXDOMAIN — no A/AAAA record published
  tls_version: null
- cert_issuer: Let's Encrypt YR2
  cert_not_after: '2026-11-19'
  cert_subject: CN=ultrasafenuclear.com
  host: ultrasafenuclear.com
  hsts: true
  hsts_max_age: 15552000
  http_status: 200
  https: true
  ownership: unverified
  reachable: true
  server: Squarespace
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ultra Safe Nuclear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ultra Safe Nuclear, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ultra Safe Nuclear
provider_slug: ultra-safe-nuclear
slug: ultra-safe-nuclear-domain-security
source_filename: ultra-safe-nuclear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: dig (8.8.8.8) + TLS handshake + HTTP HEAD, 2026-09-01\nnote: >-\n  Probed the company's primary corporate domain (usnc.com) and the one reachable\n  name-adjacent domain (ultrasafenuclear.com, ownership unverified). usnc.com publishes no\n  address record, so there is no host to test for TLS/HSTS; its mail plane is still\n  configured on the Microsoft 365 US Government cloud with a quarantine DMARC policy, which\n  is the clearest single signal that the entity was wound down rather than migrated.\nhosts:\n  - host: usnc.com\n    https: false\n    reachable: false\n    reason: NXDOMAIN — no A/AAAA record published\n    tls_version: null\n    hsts: null\n  - host: ultrasafenuclear.com\n    https: true\n    reachable: true\n    http_status: 200\n    server: Squarespace\n    tls_version: TLSv1.3\n    cert_subject: CN=ultrasafenuclear.com\n    cert_issuer: \"Let's Encrypt YR2\"\n    cert_not_after: '2026-11-19'\n    hsts: true\n \
  \   hsts_max_age: 15552000\n    ownership: unverified\ndomains:\n  - domain: usnc.com\n    registrar: GoDaddy Online Services Cayman Islands Ltd.\n    registry_expiry: '2027-03-12'\n    nameservers: [ns27.domaincontrol.com, ns28.domaincontrol.com]\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 include:spf.protection.office365.us -all'\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_record: 'v=DMARC1; p=quarantine; pct=100; rua=mailto:dmarc@usnc.com; ruf=mailto:dmarc@usnc.com; fo=1'\n    mx: ['usnctech.mail.protection.office365.us']\n    web_presence: false\n  - domain: ultrasafenuclear.com\n    registrar: null\n    created: '2022-03-30'\n    registry_expiry: '2032-03-30'\n    nameservers: [ns-cloud-b1.googledomains.com, ns-cloud-b2.googledomains.com, ns-cloud-b3.googledomains.com, ns-cloud-b4.googledomains.com]\n    dnssec: true\n    caa: []\n    spf: false\n    dmarc: false\n    mx: []\n    web_presence: placeholder\n    ownership: unverified\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ultra-safe-nuclear/refs/heads/main/security/ultra-safe-nuclear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Nuclear
- Advanced Reactors
- Small Modular Reactors
- Nuclear Fuel
- Space
- Manufacturing
- Defunct
---
