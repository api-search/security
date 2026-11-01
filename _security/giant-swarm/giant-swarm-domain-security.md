---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@giantswarm.io"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: giantswarm.io
  spf: true
hosts:
- cert_expires: Dec  8 05:53:24 2026 GMT
  host: giantswarm.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Giant Swarm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Giant Swarm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Giant Swarm
provider_slug: giant-swarm
slug: giant-swarm-domain-security
source_filename: giant-swarm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: giantswarm.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 05:53:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: giantswarm.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@giantswarm.io\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/giant-swarm/security/giant-swarm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Kubernetes
- Platform Engineering
- Cloud-Native
- Observability
- Developer Platform
- Multi-Cloud
---
