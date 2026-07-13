---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mrisoftware.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: whosonlocation.com
  spf: true
hosts:
- cert_expires: Sep 22 03:07:29 2026 GMT
  host: www.mrisoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:01:45 2026 GMT
  host: apidocs.whosonlocation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: login.whosonlocation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mri Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MRI Software, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MRI Software
provider_slug: mri-software
slug: mri-software-domain-security
source_filename: mri-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mrisoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:07:29 2026 GMT\n  hsts: false\n- host: apidocs.whosonlocation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:01:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: login.whosonlocation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mrisoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: whosonlocation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mri-software/refs/heads/main/security/mri-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Management
- Investment Management
- Lease Accounting
- Facilities Management
- Commercial Real Estate
- Visitor Management
- PropTech
---
