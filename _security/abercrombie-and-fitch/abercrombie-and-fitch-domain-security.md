---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: abercrombie.com
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.abercrombie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 17:45:06 2026 GMT
  host: corporate.abercrombie.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abercrombie And Fitch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abercrombie and Fitch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Abercrombie and Fitch
provider_slug: abercrombie-and-fitch
slug: abercrombie-and-fitch-domain-security
source_filename: abercrombie-and-fitch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abercrombie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: corporate.abercrombie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:45:06 2026 GMT\n  hsts: false\ndomains:\n- domain: abercrombie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abercrombie-and-fitch/refs/heads/main/security/abercrombie-and-fitch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Retail
- Fashion
- E-commerce
- Apparel
- Lifestyle
---
