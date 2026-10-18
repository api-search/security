---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dataneuron.ai
  spf: false
hosts:
- cert_expires: Feb 12 16:34:28 2027 GMT
  host: dataneuron.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dataneuron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataNeuron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: DataNeuron
provider_slug: dataneuron
slug: dataneuron-domain-security
source_filename: dataneuron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataneuron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 16:34:28 2027 GMT\n  hsts: null\ndomains:\n- domain: dataneuron.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataneuron/refs/heads/main/security/dataneuron-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- No-Code
- LLM
- Data Annotation
- Enterprise
---
