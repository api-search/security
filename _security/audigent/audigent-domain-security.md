---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: audigent.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prebid.org
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: ad.gt
  note: ad.gt is the primary API/identity domain (id./seg./analytics.hadron.ad.gt, ids.ad.gt, a.ad.gt, p.ad.gt) and has no SPF, no DMARC, no CAA and no DNSSEC.
  spf: false
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: hadronid.net
  spf: true
  spf_record: v=spf1 include:_spf.mailersend.net ~all
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: audigent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 08:30:18 2026 GMT
  host: docs.prebid.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:54:29 2026 GMT
  host: id.hadron.ad.gt
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: seg.hadron.ad.gt
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: analytics.hadron.ad.gt
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: cdn.hadronid.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: p.ad.gt
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.audigent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Audigent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audigent, probed live across 8 host(s) and 4 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Audigent
provider_slug: audigent
slug: audigent-domain-security
source_filename: audigent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audigent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.prebid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 08:30:18 2026 GMT\n  hsts: false\n- host: id.hadron.ad.gt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:54:29 2026 GMT\n  hsts: null\n- host: seg.hadron.ad.gt\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n- host: analytics.hadron.ad.gt\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n- host: cdn.hadronid.net\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n- host: p.ad.gt\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n- host: api.audigent.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\ndomains:\n- domain: audigent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n- domain: prebid.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ad.gt\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  note: >-\n    ad.gt is the primary API/identity domain (id./seg./analytics.hadron.ad.gt,\n    ids.ad.gt, a.ad.gt, p.ad.gt) and has no SPF, no DMARC, no CAA and no DNSSEC.\n- domain: hadronid.net\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.mailersend.net ~all\n  dmarc: false\n  dmarc_policy: null\n\nx-notes:\n  hosts_supplemental_method: >-\n    audigent.com, docs.prebid.org and id.hadron.ad.gt were written by\n    0-working/probe-domain-security.py from the apis.yml hosts. The remaining\n    hosts and the ad.gt / hadronid.net domain rows were probed by hand on\n    2026-08-06 (openssl s_client + dig) because they are reachable only through\n    the client-side hadron.js bundle and are not apis.yml baseURL hosts.\n  findings:\n  - TLS 1.3 everywhere;\
  \ no plaintext or downgraded host found.\n  - HSTS is set on audigent.com only; none of the API or CDN hosts assert it.\n  - No CAA record on any domain, and no DNSSEC on any domain.\n  - >-\n    docs.prebid.org / prebid.org are third-party rows: Audigent's developer\n    documentation lives on the Prebid project's host, not its own, so those two\n    rows describe Prebid's posture rather than Audigent's.\n  - See conformance/audigent-conformance.yml for the RFC 9116 security.txt miss.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audigent/refs/heads/main/security/audigent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Data
- Identity
- Programmatic
- Audience
- Marketing
- Privacy
- Prebid
- Header Bidding
- Data Curation
---
