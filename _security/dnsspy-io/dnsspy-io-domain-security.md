---
api_specs:
- filename: dnsspy-io-openapi-generated.yml
  format: yaml
  label: DNS Spy API
  slug: dnsspy-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dnsspy-io/openapi/_ae-authored/dnsspy-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dnsspy.io
  spf: true
hosts:
- cert_expires: Jan 30 05:22:07 2027 GMT
  host: dnsspy.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dnsspy Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNS Spy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DNS Spy
provider_slug: dnsspy-io
slug: dnsspy-io-domain-security
source_filename: dnsspy-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dnsspy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 05:22:07 2027 GMT\n  hsts: false\ndomains:\n- domain: dnsspy.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dnsspy-io/security/dnsspy-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DNS
- Monitoring
- Security
- MSP
---
