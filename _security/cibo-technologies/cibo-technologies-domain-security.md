---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cibo.org
  spf: true
hosts:
- cert_expires: Nov 10 02:53:37 2026 GMT
  host: cibo.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cibo Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CIBO Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CIBO Technologies
provider_slug: cibo-technologies
slug: cibo-technologies-domain-security
source_filename: cibo-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cibo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 02:53:37 2026 GMT\n  hsts: false\ndomains:\n- domain: cibo.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cibo-technologies/refs/heads/main/security/cibo-technologies-domain-security.yml
summary_line: TLSv1.3
tags:
- Energy
- Membership
- Advocacy
- Sustainability
- Industry
---
