---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jakarta.ee
  spf: false
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eclipse.org
  spf: true
hosts:
- cert_expires: Sep 25 01:24:39 2026 GMT
  host: jakarta.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: projects.eclipse.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: cxf.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jax Ws Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JAX-WS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: JAX-WS
provider_slug: jax-ws
slug: jax-ws-domain-security
source_filename: jax-ws-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jakarta.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:24:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: projects.eclipse.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cxf.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jakarta.ee\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: eclipse.org\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jax-ws/refs/heads/main/security/jax-ws-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Jakarta EE
- Java
- JAX-WS
- SOAP
- Standard
- Web Services
- XML
---
