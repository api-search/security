---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: adagasolutions.lu
  spf: true
hosts:
- cert_expires: Jan  7 21:28:13 2027 GMT
  host: adagasolutions.lu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adagasolutions Lu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for adagasolutions-lu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: adagasolutions-lu
provider_slug: adagasolutions-lu
slug: adagasolutions-lu-domain-security
source_filename: adagasolutions-lu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adagasolutions.lu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 21:28:13 2027 GMT\n  hsts: false\ndomains:\n- domain: adagasolutions.lu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/adagasolutions-lu/security/adagasolutions-lu-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Full-stack Development
- Artificial Intelligence
- SaaS
- Luxembourg
- API Provider
---
