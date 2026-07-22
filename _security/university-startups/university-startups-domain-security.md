---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: university-startups.com
  spf: true
hosts:
- cert_expires: Jan 10 22:15:44 2027 GMT
  host: university-startups.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Startups Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University Startups, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University Startups
provider_slug: university-startups
slug: university-startups-domain-security
source_filename: university-startups-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: university-startups.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 22:15:44 2027 GMT\n  hsts: null\ndomains:\n- domain: university-startups.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-startups/refs/heads/main/security/university-startups-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- EdTech
- Special Education
- Artificial Intelligence
- Transition Planning
- IEP
- Compliance
- K-12
---
