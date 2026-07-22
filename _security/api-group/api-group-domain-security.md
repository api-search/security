---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: apigroupcorp.com
  spf: true
hosts:
- cert_expires: Sep  9 16:13:46 2026 GMT
  host: www.apigroupcorp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APi Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: APi Group
provider_slug: api-group
slug: api-group-domain-security
source_filename: api-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apigroupcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:13:46 2026 GMT\n  hsts: null\ndomains:\n- domain: apigroupcorp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-group/refs/heads/main/security/api-group-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fortune 500
- Safety Services
- Industrial Services
- Specialty Services
- Contracting
---
