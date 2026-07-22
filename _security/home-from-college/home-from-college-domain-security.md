---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: homefromcollege.com
  spf: true
hosts:
- cert_expires: Aug 26 09:37:00 2026 GMT
  host: www.homefromcollege.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Home From College Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Home From College, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Home From College
provider_slug: home-from-college
slug: home-from-college-domain-security
source_filename: home-from-college-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.homefromcollege.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 09:37:00 2026 GMT\n  hsts: false\ndomains:\n- domain: homefromcollege.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/home-from-college/refs/heads/main/security/home-from-college-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Marketplace
- Gen Z
- Creator Economy
- Gig Economy
- Students
- Marketing
- Influencer Marketing
---
