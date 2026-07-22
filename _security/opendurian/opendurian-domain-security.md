---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opendurian.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: opendurian.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Opendurian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenDurian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenDurian
provider_slug: opendurian
slug: opendurian-domain-security
source_filename: opendurian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendurian.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: opendurian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendurian/refs/heads/main/security/opendurian-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Education
- EdTech
- Test Preparation
- Language Learning
- E-Learning
- Thailand
- Online Courses
---
