---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apicur.io
  spf: false
hosts:
- cert_expires: Sep 27 09:28:52 2026 GMT
  host: www.apicur.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apicurio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apicurio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Apicurio
provider_slug: apicurio
slug: apicurio-domain-security
source_filename: apicurio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apicur.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:28:52 2026 GMT\n  hsts: false\ndomains:\n- domain: apicur.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/security/apicurio-domain-security.yml
summary_line: TLSv1.3
tags:
- Apache License
- API Design
- API Registry
- Avro
- AsyncAPI
- Java
- Open Source
- OpenAPI
- Red Hat
- Schema Registry
---
