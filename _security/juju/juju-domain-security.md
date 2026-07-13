---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: juju.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: www.juju.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Juju Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juju, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Juju
provider_slug: juju
slug: juju-domain-security
source_filename: juju-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.juju.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: juju.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juju/refs/heads/main/security/juju-domain-security.yml
summary_line: TLSv1.2
tags:
- Jobs
- Public APIs
---
