---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: energytransferequity.com
  mx: []
  nameservers:
  - ns1.namefind.com
  - ns2.namefind.com
  note: 'SPF is a hard-fail null record and there are no MX records — the parking operator has disabled mail on the domain. The _dmarc TXT lookup returns the apex "v=spf1 -all" string, i.e. a wildcard TXT answer, NOT a DMARC policy; recorded as dmarc: false so a wildcard is not miscounted as a published policy.'
  spf: true
  spf_record: v=spf1 -all
hosts:
- cert_issuer: GoDaddy TLS Intermediate CA DV - R1v1
  cert_not_after: '2027-01-30'
  cert_not_before: '2026-07-16'
  cert_subject: CN=energytransferequity.com
  cipher: TLS_AES_128_GCM_SHA256
  company_controlled: false
  host: energytransferequity.com
  hsts: false
  hsts_max_age: null
  https: true
  note: GoDaddy aftermarket parking lander; answers 200 on every path
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Energy Transfer Equity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Energy Transfer Equity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Energy Transfer Equity
provider_slug: energy-transfer-equity
slug: energy-transfer-equity-domain-security
source_filename: energy-transfer-equity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  dig (A/NS/DS/CAA/TXT/MX) plus an OpenSSL TLS handshake and an HTTP HEAD against\n  energytransferequity.com, the legacy Energy Transfer Equity, L.P. corporate\n  domain. 0-working/probe-domain-security.py returned \"no-hosts\" for this slug\n  because apis.yml carries no Website property and no apis[] baseURL — the record\n  is a defunct-entity index — so the legacy domain was probed by hand.\nnote: >-\n  FINDING: the legacy corporate domain is no longer under company control. It is\n  delegated to GoDaddy NameFind parking nameservers and is listed for sale on the\n  GoDaddy aftermarket. The TLS certificate is a GoDaddy DV cert issued to the\n  parking service, not an Energy Transfer certificate. Recorded because a lapsed\n  corporate domain that answers 200 to everything is a live impersonation surface\n  for a Fortune 100 name, and because it is why every /.well-known/ probe on that\n  host must be discarded. The successor\
  \ entity's hosts (energytransfer.com,\n  dev.messenger.energytransfer.com) are profiled in all/energy-transfer/ and are\n  deliberately NOT scored here.\nhosts:\n  - host: energytransferequity.com\n    https: true\n    tls_version: TLSv1.3\n    cipher: TLS_AES_128_GCM_SHA256\n    cert_subject: CN=energytransferequity.com\n    cert_issuer: GoDaddy TLS Intermediate CA DV - R1v1\n    cert_not_before: '2026-07-16'\n    cert_not_after: '2027-01-30'\n    hsts: false\n    hsts_max_age: null\n    company_controlled: false\n    note: GoDaddy aftermarket parking lander; answers 200 on every path\ndomains:\n  - domain: energytransferequity.com\n    nameservers: [ns1.namefind.com, ns2.namefind.com]\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: v=spf1 -all\n    dmarc: false\n    dmarc_policy: null\n    mx: []\n    note: >-\n      SPF is a hard-fail null record and there are no MX records — the parking\n      operator has disabled mail on the domain. The _dmarc TXT lookup returns the\n\
  \      apex \"v=spf1 -all\" string, i.e. a wildcard TXT answer, NOT a DMARC policy;\n      recorded as dmarc: false so a wildcard is not miscounted as a published\n      policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energy-transfer-equity/refs/heads/main/security/energy-transfer-equity-domain-security.yml
summary_line: TLSv1.3
tags:
- Energy
- Pipelines
- Midstream
- Defunct Entity
- Fortune 100
---
