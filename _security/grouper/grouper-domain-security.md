---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hellogrouper.com
  spf: true
hosts:
- cert_expires: Sep 12 22:36:54 2026 GMT
  host: hellogrouper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grouper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grouper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Grouper
provider_slug: grouper
slug: grouper-domain-security
source_filename: grouper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hellogrouper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 22:36:54 2026 GMT\n  hsts: false\ndomains:\n- domain: hellogrouper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grouper/refs/heads/main/security/grouper-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthy Aging
- Health and Wellness
- Older Adults
- Medicare Advantage
- Social Connection
- Membership
- Consumer Health
---
