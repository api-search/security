---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: liftaven.com
  spf: true
hosts:
- cert_expires: Feb  2 19:52:32 2027 GMT
  host: liftaven.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LiftSEO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiftSEO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LiftSEO
provider_slug: liftaven-com
slug: liftaven-com-domain-security
source_filename: liftaven-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liftaven.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 19:52:32 2027 GMT\n  hsts: false\ndomains:\n- domain: liftaven.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/liftaven-com/security/liftaven-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SEO
- Artificial Intelligence
- Marketing
- Analytics
- Automation
---
