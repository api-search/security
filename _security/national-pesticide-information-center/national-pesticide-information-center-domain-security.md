---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: orst.edu
  spf: true
hosts:
- cert_expires: Sep 21 07:26:33 2026 GMT
  host: npic.orst.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Pesticide Information Center Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Pesticide Information Center, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Pesticide Information Center
provider_slug: national-pesticide-information-center
slug: national-pesticide-information-center-domain-security
source_filename: national-pesticide-information-center-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: npic.orst.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:26:33 2026 GMT\n  hsts: false\ndomains:\n- domain: orst.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-pesticide-information-center/refs/heads/main/security/national-pesticide-information-center-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Environment
- Federal Government
- Pesticides
- Public Health
---
