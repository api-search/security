---
api_specs:
- filename: isovalent-cilium-agent-openapi.yml
  format: yaml
  label: Cilium Agent API
  slug: cilium-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isovalent/refs/heads/main/openapi/isovalent-cilium-agent-openapi.yml
- filename: isovalent-cilium-health-openapi.yml
  format: yaml
  label: Cilium Health API
  slug: cilium-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isovalent/refs/heads/main/openapi/isovalent-cilium-health-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: isovalent.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cilium.io
  spf: true
hosts:
- cert_expires: Sep 17 08:43:48 2026 GMT
  host: isovalent.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:32:49 2026 GMT
  host: docs.cilium.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: hubble-relay.kube-system.svc.cluster.local
  https: false
kind: domain-security
layout: security
method: probed
name: Isovalent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Isovalent, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Isovalent
provider_slug: isovalent
slug: isovalent-domain-security
source_filename: isovalent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isovalent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.cilium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:32:49 2026 GMT\n  hsts: false\n- host: hubble-relay.kube-system.svc.cluster.local\n  https: false\ndomains:\n- domain: isovalent.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cilium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isovalent/refs/heads/main/security/isovalent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Networking
- Kubernetes
- eBPF
- Security
- Observability
- Cloud Native
- Service Mesh
- CNI
- Container Networking
---
