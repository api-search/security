---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: plan4all.eu
  spf: true
hosts:
- cert_expires: Dec 29 00:56:02 2026 GMT
  host: www.plan4all.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Plan4All Z S Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plan4All z.s., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Plan4All z.s.
provider_slug: plan4all-z-s
slug: plan4all-z-s-domain-security
source_filename: plan4all-z-s-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plan4all.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 00:56:02 2026 GMT\n  hsts: false\ndomains:\n- domain: plan4all.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/plan4all-z-s/security/plan4all-z-s-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Financial-Planning
- API
- EU
---
