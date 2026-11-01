---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: technicalcommunities.com
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: www.technicalcommunities.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Technical Communities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Technical Communities, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Technical Communities
provider_slug: technical-communities
slug: technical-communities-domain-security
source_filename: technical-communities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.technicalcommunities.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: technicalcommunities.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/technical-communities/security/technical-communities-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Reseller
- Marketing
- GSA
- Distribution
---
