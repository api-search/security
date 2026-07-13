---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: websitecarbon.com
  spf: false
hosts:
- cert_expires: Sep 10 14:18:42 2026 GMT
  host: api.websitecarbon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Website Carbon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Website Carbon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Website Carbon
provider_slug: website-carbon
slug: website-carbon-domain-security
source_filename: website-carbon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.websitecarbon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:18:42 2026 GMT\n  hsts: false\ndomains:\n- domain: websitecarbon.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/website-carbon/refs/heads/main/security/website-carbon-domain-security.yml
summary_line: TLSv1.3
tags:
- Environment
- Public APIs
---
