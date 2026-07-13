---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: avoindata.fi
  spf: false
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: www.avoindata.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Open Government Finland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Finland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Open Government, Finland
provider_slug: open-government-finland
slug: open-government-finland-domain-security
source_filename: open-government-finland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avoindata.fi\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avoindata.fi\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-finland/refs/heads/main/security/open-government-finland-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC
tags:
- Government
- Public APIs
---
