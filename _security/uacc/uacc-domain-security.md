---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unitedautocredit.net
  spf: true
hosts:
- cert_expires: Dec 15 08:36:51 2026 GMT
  host: unitedautocredit.net
  hsts: true
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: United Auto Credit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Auto Credit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: United Auto Credit
provider_slug: uacc
slug: uacc-domain-security
source_filename: uacc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unitedautocredit.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 08:36:51 2026 GMT\n  hsts: true\ndomains:\n- domain: unitedautocredit.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/uacc/security/uacc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Auto
- Lending
- Non-prime
- California
---
