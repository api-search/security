---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: humanfn.com
  spf: true
hosts:
- cert_expires: Jan  2 22:53:06 2027 GMT
  host: humanfn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HumanFn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HumanFn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HumanFn
provider_slug: humanfn-com
slug: humanfn-com-domain-security
source_filename: humanfn-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanfn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 22:53:06 2027 GMT\n  hsts: false\ndomains:\n- domain: humanfn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/humanfn-com/security/humanfn-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Services
- Legal
- OnSite
- Automation
- Platform
---
