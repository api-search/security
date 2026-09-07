---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: cleanshelf.com
  mx: []
  nameservers:
  - nsp1.sap.de
  - nsp3.sap.net
  - nsp4.sap.asia
  spf: true
  spf_record: v=spf1 mx ip4:155.56.68.0/24
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leanix.net
  spf: true
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  cert_subject: C=DE, ST=Baden-Wuerttemberg, L=Walldorf, O=SAP SE, CN=leanix.info
  host: cleanshelf.com
  hsts: false
  http_status: 301
  https: true
  redirects_to: https://www.leanix.net/
  tls_version: TLSv1.3
- host: www.cleanshelf.com
  hsts: false
  http_status: 301
  https: true
  redirects_to: https://www.leanix.net/
  tls_version: TLSv1.3
- cert_expires: Nov 19 01:08:54 2026 GMT
  host: www.leanix.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Successor host; scored on the leanix record, recorded here for the redirect chain only.
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cleanshelf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cleanshelf, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cleanshelf
provider_slug: cleanshelf
slug: cleanshelf-domain-security
source_filename: cleanshelf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of cleanshelf.com — the only domain Cleanshelf ever\n  operated — plus www.leanix.net, the successor host cleanshelf.com now\n  redirects to. A prior round of this artifact probed zylo.com, which was a\n  misattribution: Cleanshelf was acquired by LeanIX, not Zylo.\nnote: >-\n  The cleanshelf.com certificate is issued to O=SAP SE, CN=leanix.info and the\n  domain's nameservers are nsp1.sap.de / nsp3.sap.net / nsp4.sap.asia, which is\n  direct evidence the domain is operated by SAP through LeanIX. The domain\n  serves no HSTS header, publishes no CAA, no DS (DNSSEC) and no DMARC record,\n  and has no MX — consistent with a retained redirect domain rather than an\n  operating property.\nhosts:\n- host: cleanshelf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_subject: C=DE, ST=Baden-Wuerttemberg,\
  \ L=Walldorf, O=SAP SE, CN=leanix.info\n  hsts: false\n  http_status: 301\n  redirects_to: https://www.leanix.net/\n- host: www.cleanshelf.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  http_status: 301\n  redirects_to: https://www.leanix.net/\n- host: www.leanix.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 01:08:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Successor host; scored on the leanix record, recorded here for the redirect chain only.\ndomains:\n- domain: cleanshelf.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 mx ip4:155.56.68.0/24\n  dmarc: false\n  dmarc_policy: null\n  mx: []\n  nameservers:\n  - nsp1.sap.de\n  - nsp3.sap.net\n  - nsp4.sap.asia\n- domain: leanix.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cleanshelf/refs/heads/main/security/cleanshelf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Acquired
- License Management
- SaaS Management
- Shadow IT
- SMP
- Software Asset Management
- Spend Optimization
---
