---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atxminisplit.com
  spf: true
hosts:
- cert_expires: Dec 31 16:51:04 2026 GMT
  host: atxminisplit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ATX Mini Split Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ATX Mini Split, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ATX Mini Split
provider_slug: atxminisplit-com
slug: atxminisplit-com-domain-security
source_filename: atxminisplit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atxminisplit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 16:51:04 2026 GMT\n  hsts: false\ndomains:\n- domain: atxminisplit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/atxminisplit-com/security/atxminisplit-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- HVAC
- Mini-split
- Austin
- Rankings
- Data
---
