---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: getdocket.com
  spf: true
hosts:
- cert_expires: Sep  4 21:21:55 2026 GMT
  host: getdocket.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docket Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docket Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Docket Technologies
provider_slug: docket-technologies
slug: docket-technologies-domain-security
source_filename: docket-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getdocket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 21:21:55 2026 GMT\n  hsts: null\ndomains:\n- domain: getdocket.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docket-technologies/refs/heads/main/security/docket-technologies-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
---
