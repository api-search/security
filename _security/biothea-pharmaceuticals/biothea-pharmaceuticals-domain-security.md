---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biotheapharma.com
  spf: true
hosts:
- cert_expires: Mar 31 22:06:39 2027 GMT
  host: www.biotheapharma.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biothea Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biothea Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Biothea Pharmaceuticals
provider_slug: biothea-pharmaceuticals
slug: biothea-pharmaceuticals-domain-security
source_filename: biothea-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biotheapharma.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 31 22:06:39 2027 GMT\n  hsts: false\ndomains:\n- domain: biotheapharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biothea-pharmaceuticals/refs/heads/main/security/biothea-pharmaceuticals-domain-security.yml
summary_line: TLSv1.2
tags:
- Biotech
- Pharmaceuticals
- Healthcare
- Anaphylaxis
- NeedleFree
---
