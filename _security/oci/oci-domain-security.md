---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencontainers.org
  spf: false
hosts:
- cert_expires: Sep 25 06:21:26 2026 GMT
  host: opencontainers.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OCI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OCI
provider_slug: oci
slug: oci-domain-security
source_filename: oci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencontainers.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 06:21:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opencontainers.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oci/refs/heads/main/security/oci-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Containers
- OCI
- Open Source
- Standards
---
