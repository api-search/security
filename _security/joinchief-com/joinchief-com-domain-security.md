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
- cert_expires: Jan  8 09:55:39 2027 GMT
  host: www.joinchief.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joinchief Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chief, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chief
provider_slug: joinchief-com
slug: joinchief-com-domain-security
source_filename: joinchief-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinchief.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 09:55:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joinchief.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/joinchief-com/security/joinchief-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Membership
- Community
- WomenLeadership
- Platform
---
