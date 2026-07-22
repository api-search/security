---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: franklinresources.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: franklintempleton.com
  spf: true
hosts:
- cert_expires: Aug 12 08:18:39 2026 GMT
  host: www.franklinresources.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 19:17:12 2026 GMT
  host: www.franklintempleton.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Franklin Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Franklin Resources, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Franklin Resources
provider_slug: franklin-resources
slug: franklin-resources-domain-security
source_filename: franklin-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.franklinresources.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 08:18:39 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.franklintempleton.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: franklinresources.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: franklintempleton.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/franklin-resources/refs/heads/main/security/franklin-resources-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fortune 500
- Investment Management
- Asset Management
- Financial Services
---
