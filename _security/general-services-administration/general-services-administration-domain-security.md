---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
  - 0 issue "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gsa.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sftool.gov
  spf: true
hosts:
- cert_expires: Aug 20 10:21:32 2026 GMT
  host: open.gsa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.gsa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: sftool.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: General Services Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for General Services Administration, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: General Services Administration
provider_slug: general-services-administration
slug: general-services-administration-domain-security
source_filename: general-services-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.gsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.gsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sftool.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gsa.gov\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sftool.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-services-administration/refs/heads/main/security/general-services-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Procurement
- Acquisition
- Open Data
---
