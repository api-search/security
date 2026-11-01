---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: textmarketer.co.uk
  spf: true
hosts:
- cert_expires: Dec 31 06:17:52 2026 GMT
  host: textmarketer.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Textmarketer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Text Marketer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Text Marketer
provider_slug: textmarketer
slug: textmarketer-domain-security
source_filename: textmarketer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: textmarketer.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 06:17:52 2026 GMT\n  hsts: false\ndomains:\n- domain: textmarketer.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/textmarketer/security/textmarketer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SMS
- Marketing
- UK
- Business
- Communications
---
