---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: brandpresence.dev
  spf: false
hosts:
- cert_expires: Jan 26 22:46:00 2027 GMT
  host: brandpresence.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BrandPresence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrandPresence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: BrandPresence
provider_slug: brandpresence-dev
slug: brandpresence-dev-domain-security
source_filename: brandpresence-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandpresence.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 22:46:00 2027 GMT\n  hsts: false\ndomains:\n- domain: brandpresence.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/brandpresence-dev/security/brandpresence-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Artificial Intelligence
- Monitoring
- Search
- Visibility
---
