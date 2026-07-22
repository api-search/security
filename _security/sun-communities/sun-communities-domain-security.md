---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: suninc.com
  spf: true
hosts:
- cert_expires: Oct  4 07:16:19 2026 GMT
  host: suninc.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sun Communities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sun Communities, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sun Communities
provider_slug: sun-communities
slug: sun-communities-domain-security
source_filename: sun-communities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suninc.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 07:16:19 2026 GMT\n  hsts: null\ndomains:\n- domain: suninc.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sun-communities/refs/heads/main/security/sun-communities-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Real Estate
- Manufactured Housing
- RV Resorts
- Marinas
- REIT
---
