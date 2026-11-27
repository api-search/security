---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: getfndtn.com
  spf: true
hosts:
- cert_expires: Dec 10 08:20:40 2026 GMT
  host: getfndtn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Foundation
provider_slug: getfndtn-com
slug: getfndtn-com-domain-security
source_filename: getfndtn-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getfndtn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 08:20:40 2026 GMT\n  hsts: false\ndomains:\n- domain: getfndtn.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getfndtn-com/security/getfndtn-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Business
- Artificial Intelligence
- Feasibility
- Planning
- Free
- Company
---
