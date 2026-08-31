---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: proactis.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: proactiscloud.com
  spf: true
hosts:
- cert_expires: Oct 12 03:45:15 2026 GMT
  host: www.proactis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:45:15 2026 GMT
  host: docs.proactis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: apiuk.proactiscloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proactis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proactis, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Proactis
provider_slug: proactis
slug: proactis-domain-security
source_filename: proactis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proactis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:45:15 2026 GMT\n  hsts: null\n- host: docs.proactis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:45:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apiuk.proactiscloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: proactis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: proactiscloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proactis/refs/heads/main/security/proactis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Procurement
- Purchase-To-Pay
- Source-To-Pay
- Spend Management
- Contract Management
- eInvoicing
- Accounts Payable
- Supplier Management
- eSourcing
- cXML
- UBL
- SCIM
---
