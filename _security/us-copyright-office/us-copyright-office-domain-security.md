---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: copyright.gov
  spf: true
hosts:
- cert_expires: Sep 25 17:56:49 2026 GMT
  host: www.copyright.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 12:52:26 2026 GMT
  host: publicrecords.copyright.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 17:56:49 2026 GMT
  host: licensing.copyright.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Copyright Office Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Copyright Office, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: US Copyright Office
provider_slug: us-copyright-office
slug: us-copyright-office-domain-security
source_filename: us-copyright-office-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.copyright.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:56:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: publicrecords.copyright.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:52:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: licensing.copyright.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:56:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: copyright.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-copyright-office/refs/heads/main/security/us-copyright-office-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Copyright
- Federal Government
- Intellectual Property
- Open Data
---
