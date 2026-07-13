---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jsph.pl
  spf: true
hosts:
- cert_expires: Aug 11 15:01:03 2026 GMT
  host: uselessfacts.jsph.pl
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Random Useless Facts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Random Useless Facts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Random Useless Facts
provider_slug: random-useless-facts
slug: random-useless-facts-domain-security
source_filename: random-useless-facts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uselessfacts.jsph.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 15:01:03 2026 GMT\n  hsts: null\ndomains:\n- domain: jsph.pl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/random-useless-facts/refs/heads/main/security/random-useless-facts-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Entertainment
- Public APIs
---
