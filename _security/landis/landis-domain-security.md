---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: landis.com
  spf: true
hosts:
- cert_expires: Sep 28 13:06:41 2026 GMT
  host: landis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Landis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Landis
provider_slug: landis
slug: landis-domain-security
source_filename: landis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: landis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:06:41 2026 GMT\n  hsts: false\ndomains:\n- domain: landis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landis/refs/heads/main/security/landis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Real Estate
- Proptech
- Fintech
- Mortgage
- Rent to Own
- Homeownership
- Housing
---
