---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: grassrootsunwired.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: grassrootsunwired.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grassroots Unwired Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grassroots Unwired, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Grassroots Unwired
provider_slug: grassroots-unwired
slug: grassroots-unwired-domain-security
source_filename: grassroots-unwired-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grassrootsunwired.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: grassrootsunwired.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grassroots-unwired/refs/heads/main/security/grassroots-unwired-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fundraising
- Nonprofit
- Political Campaigns
- Canvassing
- Advocacy
- Field Organizing
- Peer-to-Peer Texting
- Event Management
- Mobile
---
