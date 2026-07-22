---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: expedia.com
  spf: true
hosts:
- cert_expires: Aug 28 18:41:21 2026 GMT
  host: www.expedia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expedia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Expedia
provider_slug: expedia
slug: expedia-domain-security
source_filename: expedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.expedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 18:41:21 2026 GMT\n  hsts: null\ndomains:\n- domain: expedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expedia/refs/heads/main/security/expedia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Flights
- Hotels
- Lodging
- Travel
- Fortune 500
---
