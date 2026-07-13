---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gunpolicy.org
  spf: true
hosts:
- cert_expires: Aug 24 04:49:43 2026 GMT
  host: www.gunpolicy.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gun Policy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gun Policy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gun Policy
provider_slug: gun-policy
slug: gun-policy-domain-security
source_filename: gun-policy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gunpolicy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:49:43 2026 GMT\n  hsts: null\ndomains:\n- domain: gunpolicy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gun-policy/refs/heads/main/security/gun-policy-domain-security.yml
summary_line: TLSv1.3
tags:
- Government
- Public APIs
---
