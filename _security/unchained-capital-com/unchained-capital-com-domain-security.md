---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unchained-capital.com
  spf: true
hosts:
- cert_expires: Apr 29 23:59:59 2027 GMT
  host: unchained-capital.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unchained Capital Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unchained Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unchained Capital
provider_slug: unchained-capital-com
slug: unchained-capital-com-domain-security
source_filename: unchained-capital-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unchained-capital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: unchained-capital.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/unchained-capital-com/security/unchained-capital-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Bitcoin
- Financial Services
- Custody
- Investment
- Trust
---
