---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: harley-davidson.com
  spf: true
hosts:
- cert_expires: Sep 11 15:02:17 2026 GMT
  host: www.harley-davidson.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harley Davidson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Harley-Davidson, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Harley-Davidson
provider_slug: harley-davidson
slug: harley-davidson-domain-security
source_filename: harley-davidson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.harley-davidson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:02:17 2026 GMT\n  hsts: false\ndomains:\n- domain: harley-davidson.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harley-davidson/refs/heads/main/security/harley-davidson-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Apparel
- Dealers
- Motorcycles
- Parts
- Fortune 500
---
