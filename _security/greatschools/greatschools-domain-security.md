---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greatschools.org
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.greatschools.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Greatschools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GreatSchools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GreatSchools
provider_slug: greatschools
slug: greatschools-domain-security
source_filename: greatschools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greatschools.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: greatschools.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greatschools/refs/heads/main/security/greatschools-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Schools
- Education
- Ratings
- Geolocation
---
