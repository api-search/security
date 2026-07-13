---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bytewax.io
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:infrastructure-staff@python.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: pypi.org
  spf: true
hosts:
- cert_expires: Oct  1 16:32:22 2026 GMT
  host: bytewax.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 14:51:40 2026 GMT
  host: docs.bytewax.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 04:33:07 2027 GMT
  host: pypi.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bytewax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bytewax, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bytewax
provider_slug: bytewax
slug: bytewax-domain-security
source_filename: bytewax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bytewax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 16:32:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: docs.bytewax.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:51:40 2026 GMT\n  hsts: false\n- host: pypi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:33:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bytewax.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pypi.org\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:infrastructure-staff@python.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bytewax/refs/heads/main/security/bytewax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Stream Processing
- Python
- Dataflow
- Real-Time
- Kafka
- Windowing
- Connectors
- Distributed Systems
- Kubernetes
- Open Source
---
