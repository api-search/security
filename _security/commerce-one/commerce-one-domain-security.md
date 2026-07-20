---
description: ''
domains:
- a_records:
  - 139.64.220.120
  caa: []
  dmarc: false
  dnssec: false
  domain: xcbl.org
  ds_records: []
  hsts: false
  https:
    evidence: TCP connect to xcbl.org:443 refused (errno 61); site is served over plain HTTP only.
    supported: false
  mx: []
  nameservers:
  - ns1.dotster.com
  - ns2.dotster.com
  resolves: true
  risk_notes:
  - No TLS. The xCBL 4.0 schema and sample distribution can only be downloaded over unauthenticated, unencrypted HTTP, so its integrity cannot be verified in transit. Consumers should verify the archive out of band.
  - No SPF, DMARC or MX records — the domain is not configured to send or receive mail.
  - No CAA records and no DNSSEC.
  server: Microsoft-IIS/10.0
  spf: false
  txt: []
  x_powered_by: ASP.NET
- a_records: []
  created: '1997-03-26'
  domain: commerceone.com
  registered: true
  registrar: Domain.com — Network Solutions, LLC
  registry_expiry: '2027-03-27'
  resolves: false
  risk_notes:
  - The historical corporate domain is registered and renewed but publishes no A record, so no service, mail or well-known surface exists on it. The xcblwebmaster@commerceone.com / xcblsupport@commerceone.com contacts still printed on xcbl.org are therefore not expected to be deliverable.
  status:
  - clientDeleteProhibited
- domain: commerce-one.com
  related: false
  resolves: true
  risk_notes:
  - Unrelated parked domain (GoDaddy nameservers) serving a lander redirect on every path. Not a Commerce One property; recorded only to prevent it being mistaken for one.
hosts: []
kind: domain-security
layout: security
method: probed
name: Commerce One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commerce One, probed live across 0 host(s) and 3 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Commerce One
provider_slug: commerce-one
slug: commerce-one-domain-security
source_filename: commerce-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probe, 2026-07-20\ndomains:\n  - domain: xcbl.org\n    resolves: true\n    a_records:\n      - 139.64.220.120\n    nameservers:\n      - ns1.dotster.com\n      - ns2.dotster.com\n    https:\n      supported: false\n      evidence: TCP connect to xcbl.org:443 refused (errno 61); site is served over plain HTTP only.\n    hsts: false\n    server: Microsoft-IIS/10.0\n    x_powered_by: ASP.NET\n    dnssec: false\n    ds_records: []\n    caa: []\n    spf: false\n    dmarc: false\n    mx: []\n    txt: []\n    risk_notes:\n      - >-\n        No TLS. The xCBL 4.0 schema and sample distribution can only be\n        downloaded over unauthenticated, unencrypted HTTP, so its integrity\n        cannot be verified in transit. Consumers should verify the archive out\n        of band.\n      - No SPF, DMARC or MX records — the domain is not configured to send or receive mail.\n      - No CAA records and no DNSSEC.\n  - domain:\
  \ commerceone.com\n    resolves: false\n    a_records: []\n    registered: true\n    registrar: Domain.com — Network Solutions, LLC\n    created: '1997-03-26'\n    registry_expiry: '2027-03-27'\n    status:\n      - clientDeleteProhibited\n    risk_notes:\n      - >-\n        The historical corporate domain is registered and renewed but publishes\n        no A record, so no service, mail or well-known surface exists on it. The\n        xcblwebmaster@commerceone.com / xcblsupport@commerceone.com contacts\n        still printed on xcbl.org are therefore not expected to be deliverable.\n  - domain: commerce-one.com\n    resolves: true\n    related: false\n    risk_notes:\n      - >-\n        Unrelated parked domain (GoDaddy nameservers) serving a lander redirect\n        on every path. Not a Commerce One property; recorded only to prevent it\n        being mistaken for one.\nsummary: >-\n  Commerce One has no defended domain posture. The one live host, xcbl.org, is\n  HTTP-only with no HSTS,\
  \ DNSSEC, CAA, SPF or DMARC; the historical corporate\n  domain does not resolve at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commerce-one/refs/heads/main/security/commerce-one-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- B2B
- eCommerce
- Procurement
- Supply Chain
- XML
- EDI
- Schema
- Marketplace
- Defunct
---
