---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bia.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: doi.gov
  spf: true
hosts:
- cert_expires: Aug 17 07:34:42 2026 GMT
  host: www.bia.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: biamaps.doi.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 17 07:32:43 2026 GMT
  host: www.bie.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bureau Of Indian Affairs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Indian Affairs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Indian Affairs
provider_slug: bureau-of-indian-affairs
slug: bureau-of-indian-affairs-domain-security
source_filename: bureau-of-indian-affairs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bia.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:34:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: biamaps.doi.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\n- host: www.bie.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:32:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bia.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: doi.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-indian-affairs/refs/heads/main/security/bureau-of-indian-affairs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- GIS
- ICWA
- Indigenous
- Tribal
- Tribal Governance
- Trust Assets
---
