---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: suncoast.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_phishspf.knowbe4.com include:sendgrid.net ip4:198.51.245.68 ip4:65.89.183.150 -all
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: suncoastcreditunion.com
  spf: true
hosts:
- cert_expires: Sep 28 00:35:43 2026 GMT
  host: www.suncoast.com
  hsts: null
  hsts_max_age: null
  https: true
  note: Canonical brand domain (Cloudflare-fronted). Returns HTTP 403 to non-browser clients (bot protection), so HSTS/response headers could not be read. www.suncoastcreditunion.com issues a 301 redirect here.
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:01:13 2026 GMT
  host: www.suncoastcreditunion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: Legacy domain; 301-redirects to www.suncoast.com.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suncoast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suncoast Credit Union, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Suncoast Credit Union
provider_slug: suncoast
slug: suncoast-domain-security
source_filename: suncoast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (both brand domains)\nhosts:\n- host: www.suncoast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:35:43 2026 GMT\n  hsts: null\n  hsts_max_age: null\n  note: >-\n    Canonical brand domain (Cloudflare-fronted). Returns HTTP 403 to non-browser\n    clients (bot protection), so HSTS/response headers could not be read.\n    www.suncoastcreditunion.com issues a 301 redirect here.\n- host: www.suncoastcreditunion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:01:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: Legacy domain; 301-redirects to www.suncoast.com.\ndomains:\n- domain: suncoast.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 include:spf.protection.outlook.com include:_phishspf.knowbe4.com\n    include:sendgrid.net ip4:198.51.245.68 ip4:65.89.183.150 -all\n  dmarc: true\n  dmarc_policy: reject\n\
  - domain: suncoastcreditunion.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suncoast/refs/heads/main/security/suncoast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- United States
- Credit Union
- Florida
- Open Finance
- Data Aggregation
---
