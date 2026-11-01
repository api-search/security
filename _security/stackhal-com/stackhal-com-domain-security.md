---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: stackhal.com
  spf: true
hosts:
- cert_expires: Jan 20 09:59:44 2027 GMT
  host: stackhal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stackhal Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for stackhal-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: stackhal-com
provider_slug: stackhal-com
slug: stackhal-com-domain-security
source_filename: stackhal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stackhal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 09:59:44 2027 GMT\n  hsts: false\ndomains:\n- domain: stackhal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/stackhal-com/security/stackhal-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Developer Tools
- SEO
- Infrastructure
- Open Source
---
