---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oti-labs.com
  spf: true
hosts:
- cert_expires: Jan 15 00:21:57 2027 GMT
  host: oti-labs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oti Labs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for oti-labs-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: oti-labs-com
provider_slug: oti-labs-com
slug: oti-labs-com-domain-security
source_filename: oti-labs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oti-labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 00:21:57 2027 GMT\n  hsts: false\ndomains:\n- domain: oti-labs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/oti-labs-com/security/oti-labs-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Domain-Intelligence
- Security
- WHOIS
- DNS
- SSL
---
