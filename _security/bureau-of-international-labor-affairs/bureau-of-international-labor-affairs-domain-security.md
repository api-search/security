---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dol.gov
  spf: true
hosts:
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: www.dol.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.dol.gov
  https: false
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.dol.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bureau Of International Labor Affairs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of International Labor Affairs, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of International Labor Affairs
provider_slug: bureau-of-international-labor-affairs
slug: bureau-of-international-labor-affairs-domain-security
source_filename: bureau-of-international-labor-affairs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dol.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: null\n- host: developer.dol.gov\n  https: false\n- host: api.dol.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dol.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-international-labor-affairs/refs/heads/main/security/bureau-of-international-labor-affairs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- International
- Labor
- Standards
- Child Labor
- Forced Labor
- Human Trafficking
---
