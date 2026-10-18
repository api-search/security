---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crmls.org
  spf: true
hosts:
- cert_expires: Dec 26 23:31:17 2026 GMT
  host: www.crmls.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crmls Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for California Regional MLS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: California Regional MLS
provider_slug: crmls
slug: crmls-domain-security
source_filename: crmls-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crmls.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:31:17 2026 GMT\n  hsts: false\ndomains:\n- domain: crmls.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crmls/refs/heads/main/security/crmls-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- MLS
- IDX
- RESO
- Listings
- California
---
