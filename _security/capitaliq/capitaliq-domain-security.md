---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: capitaliq.com
  spf: true
hosts:
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: www.capitaliq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capitaliq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capitaliq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Capitaliq
provider_slug: capitaliq
slug: capitaliq-domain-security
source_filename: capitaliq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capitaliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: capitaliq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitaliq/refs/heads/main/security/capitaliq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Data
- Analytics
- Market Intelligence
- Research
---
