---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: every.org
  spf: true
hosts:
- cert_expires: Oct  8 09:33:01 2026 GMT
  host: www.every.org
  hsts: unknown
  https: true
  note: www.every.org is fronted by a Vercel bot challenge and returned HTTP 429 ("Vercel Security Checkpoint") to every unauthenticated probe on 2026-08-28, so response headers could not be read. Not a finding about the provider.
  tls_version: TLSv1.3
- cert_expires: Oct 17 02:22:30 2026 GMT
  host: partners.every.org
  hsts: max-age=15552000; includeSubDomains; preload
  hsts_note: Observed directly on GET https://partners.every.org/ (HTTP 404) and on GET https://partners.every.org/v0.2/search/pets (HTTP 400). The automated probe recorded null because it only reads headers from 2xx responses; the API host answers no unauthenticated 2xx.
  https: true
  tls_version: TLSv1.3
- host: docs.every.org
  hsts: null
  https: true
  note: Docusaurus documentation host; probed 2026-08-28.
kind: domain-security
layout: security
method: probed
name: Every Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Every.org, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Every.org
provider_slug: every-org
slug: every-org-domain-security
source_filename: every-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.every.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:33:01 2026 GMT\n  hsts: unknown\n  note: >-\n    www.every.org is fronted by a Vercel bot challenge and returned HTTP 429\n    (\"Vercel Security Checkpoint\") to every unauthenticated probe on 2026-08-28,\n    so response headers could not be read. Not a finding about the provider.\n- host: partners.every.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:22:30 2026 GMT\n  hsts: max-age=15552000; includeSubDomains; preload\n  hsts_note: >-\n    Observed directly on GET https://partners.every.org/ (HTTP 404) and on\n    GET https://partners.every.org/v0.2/search/pets (HTTP 400). The automated\n    probe recorded null because it only reads headers from 2xx responses; the\n    API host answers no unauthenticated 2xx.\n- host: docs.every.org\n  https: true\n  hsts:\
  \ null\n  note: Docusaurus documentation host; probed 2026-08-28.\ndomains:\n- domain: every.org\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/every-org/refs/heads/main/security/every-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Charities
- Donations
- Fundraising
- Nonprofits
- Philanthropy
- Webhooks
- Giving
---
