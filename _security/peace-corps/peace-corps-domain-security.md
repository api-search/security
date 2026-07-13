---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: peacecorps.gov
  spf: true
hosts:
- cert_expires: Oct  5 12:46:31 2026 GMT
  host: www.peacecorps.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peace Corps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peace Corps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Peace Corps
provider_slug: peace-corps
slug: peace-corps-domain-security
source_filename: peace-corps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peacecorps.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:46:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peacecorps.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peace-corps/refs/heads/main/security/peace-corps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- International Development
- Volunteers
---
