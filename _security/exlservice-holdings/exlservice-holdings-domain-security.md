---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exlservice.com
  spf: true
hosts:
- cert_expires: Jul 24 09:32:07 2026 GMT
  host: www.exlservice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.exlservice.com
  https: false
- host: api.exlservice.com
  https: false
kind: domain-security
layout: security
method: probed
name: Exlservice Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExlService Holdings, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ExlService Holdings
provider_slug: exlservice-holdings
slug: exlservice-holdings-domain-security
source_filename: exlservice-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exlservice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 24 09:32:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.exlservice.com\n  https: false\n- host: api.exlservice.com\n  https: false\ndomains:\n- domain: exlservice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exlservice-holdings/refs/heads/main/security/exlservice-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Digital Operations
- BPO
---
