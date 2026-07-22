---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: joinchief.com
  spf: true
hosts:
- cert_expires: Sep 12 00:07:42 2026 GMT
  host: www.joinchief.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chief Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chief, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chief
provider_slug: chief
slug: chief-domain-security
source_filename: chief-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinchief.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:07:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: joinchief.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chief/refs/heads/main/security/chief-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Membership
- Executive Network
- Leadership
- Community
- Coaching
- Women in Leadership
- Professional Network
---
