---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dfree.com
  spf: true
hosts:
- cert_expires: Dec 18 21:00:26 2026 GMT
  host: dfree.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dfree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dfree, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dfree
provider_slug: dfree
slug: dfree-domain-security
source_filename: dfree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dfree.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 21:00:26 2026 GMT\n  hsts: false\ndomains:\n- domain: dfree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dfree/security/dfree-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Finance
- Education
- Community
- Wealth
---
