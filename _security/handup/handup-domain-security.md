---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: handup.org
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: handup.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Handup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HandUp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HandUp
provider_slug: handup
slug: handup-domain-security
source_filename: handup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handup.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: handup.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handup/refs/heads/main/security/handup-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Crowdfunding
- Nonprofit
- Donations
- Philanthropy
- Fundraising
- Homelessness
- Poverty
- Social Impact
---
