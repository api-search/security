---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: re3data.org
  spf: true
hosts:
- cert_expires: Dec 25 12:07:27 2026 GMT
  host: www.re3data.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Re3Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for re3data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: re3data
provider_slug: re3data
slug: re3data-domain-security
source_filename: re3data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.re3data.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 12:07:27 2026 GMT\n  hsts: false\ndomains:\n- domain: re3data.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/re3data/refs/heads/main/security/re3data-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data
- Registry
- OpenScience
- Metadata
- Research
---
