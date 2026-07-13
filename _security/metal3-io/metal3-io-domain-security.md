---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: metal3.io
  spf: false
hosts:
- cert_expires: Sep 21 19:23:53 2026 GMT
  host: metal3.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metal3 Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metal3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Metal3
provider_slug: metal3-io
slug: metal3-io-domain-security
source_filename: metal3-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metal3.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:23:53 2026 GMT\n  hsts: false\ndomains:\n- domain: metal3.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metal3-io/refs/heads/main/security/metal3-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Bare Metal
- Cloud Native
- Incubating
- Infrastructure
- Kubernetes
- Provisioning
---
