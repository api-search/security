---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: random-d.uk
  spf: true
hosts:
- cert_expires: Sep  8 05:42:14 2026 GMT
  host: random-d.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Randomduck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RandomDuck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RandomDuck
provider_slug: randomduck
slug: randomduck-domain-security
source_filename: randomduck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: random-d.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 05:42:14 2026 GMT\n  hsts: false\ndomains:\n- domain: random-d.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/randomduck/refs/heads/main/security/randomduck-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Animals
- Public APIs
---
