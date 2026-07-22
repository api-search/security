---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: recommind.com
  spf: true
hosts:
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: www.recommind.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Recommind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recommind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Recommind
provider_slug: recommind
slug: recommind-domain-security
source_filename: recommind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.recommind.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: recommind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recommind/refs/heads/main/security/recommind-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Saas
- eDiscovery
- Legal Tech
- Information Governance
- Analytics
- Machine Learning
- OpenText
---
