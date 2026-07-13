---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: globelifeinsurance.com
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.globelifeinsurance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: developer.globelifeinsurance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.globelifeinsurance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Globe Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globe Life, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Globe Life
provider_slug: globe-life
slug: globe-life-domain-security
source_filename: globe-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.globelifeinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: developer.globelifeinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\n- host: api.globelifeinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: globelifeinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globe-life/refs/heads/main/security/globe-life-domain-security.yml
summary_line: TLSv1.3
tags:
- Insurance
- Life Insurance
- Financial Services
---
