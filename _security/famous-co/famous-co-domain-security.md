---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: famous.co
  spf: true
hosts:
- cert_expires: Dec 23 08:57:54 2026 GMT
  host: famous.co
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Famous Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Famous, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Famous
provider_slug: famous-co
slug: famous-co-domain-security
source_filename: famous-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: famous.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 08:57:54 2026 GMT\n  hsts: null\ndomains:\n- domain: famous.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/famous-co/security/famous-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- APIs
- Integration
- DeveloperExperience
---
