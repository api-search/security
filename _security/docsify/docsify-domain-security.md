---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: js.org
  spf: true
hosts:
- cert_expires: Sep 29 14:27:59 2026 GMT
  host: docsify.js.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docsify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docsify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Docsify
provider_slug: docsify
slug: docsify-domain-security
source_filename: docsify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docsify.js.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:27:59 2026 GMT\n  hsts: false\ndomains:\n- domain: js.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docsify/refs/heads/main/security/docsify-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Documentation
- Static Site Generators
---
