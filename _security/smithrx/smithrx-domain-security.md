---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smithrx.com
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: mysmithrx.com
  note: no DMARC record published for the application/API domain
  spf: true
hosts:
- cert_expires: Oct 10 14:03:18 2026 GMT
  host: smithrx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: api.mysmithrx.com
  hsts: false
  https: true
  note: live API host; returns a plain-text "404 page not found" router response at every probed path (no public routes, no spec, no /.well-known)
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: member.mysmithrx.com
  hsts: false
  https: true
  note: member portal single-page app; answers 200 with an HTML shell for every path
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: partner.mysmithrx.com
  hsts: false
  https: true
  note: broker/TPA partner portal single-page app; answers 200 with an HTML shell for every path
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smithrx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmithRx, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SmithRx
provider_slug: smithrx
slug: smithrx-domain-security
source_filename: smithrx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the mysmithrx.com application\n  and API hosts discovered during contract discovery\nhosts:\n- host: smithrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 14:03:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mysmithrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: false\n  note: live API host; returns a plain-text \"404 page not found\" router response at\n    every probed path (no public routes, no spec, no /.well-known)\n- host: member.mysmithrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\n  note: member portal single-page app; answers 200 with an HTML shell for every path\n- host: partner.mysmithrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\n  note: broker/TPA partner portal single-page\
  \ app; answers 200 with an HTML shell\n    for every path\ndomains:\n- domain: smithrx.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mysmithrx.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: false\n  dmarc_policy: null\n  note: no DMARC record published for the application/API domain\nfindings:\n- HSTS is enforced on the marketing site (smithrx.com, max-age 31536000) but is absent\n  on all three mysmithrx.com application and API hosts.\n- DMARC is published for smithrx.com (p=quarantine) but not for mysmithrx.com.\n- DNSSEC is not enabled on either registrable domain.\n- CAA is published on both registrable domains.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smithrx/refs/heads/main/security/smithrx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Pharmacy
- Pharmacy Benefit Management
- Prescription Drugs
- Employee Benefits
- Claims
- Insurance
- Health Technology
---
