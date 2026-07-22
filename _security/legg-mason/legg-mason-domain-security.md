---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: franklintempleton.com
  spf: true
hosts:
- cert_expires: Sep  9 19:17:12 2026 GMT
  host: www.franklintempleton.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Legg Mason Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Legg Mason, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Legg Mason
provider_slug: legg-mason
slug: legg-mason-domain-security
source_filename: legg-mason-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.franklintempleton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: franklintempleton.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legg-mason/refs/heads/main/security/legg-mason-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Asset Management
- Investment Management
- Financial Services
- Acquired
- Franklin Templeton
- Fortune 1000
---
