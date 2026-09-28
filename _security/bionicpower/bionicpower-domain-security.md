---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bionicpower.com
  spf: true
hosts:
- cert_expires: Nov  9 22:02:24 2026 GMT
  host: www.bionicpower.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bionicpower Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bionicpower, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bionicpower
provider_slug: bionicpower
slug: bionicpower-domain-security
source_filename: bionicpower-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bionicpower.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 22:02:24 2026 GMT\n  hsts: false\ndomains:\n- domain: bionicpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bionicpower/refs/heads/main/security/bionicpower-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
