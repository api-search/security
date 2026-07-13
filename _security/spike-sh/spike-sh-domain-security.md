---
api_specs:
- filename: api.spike.sh
  format: yaml
  label: Spike.sh API
  slug: spike-sh
  spec_type: OpenAPI
  url: https://api.spike.sh
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spike.sh
  spf: true
hosts:
- cert_expires: Aug 13 17:15:24 2026 GMT
  host: spike.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:08:56 2026 GMT
  host: docs.spike.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 12:51:24 2026 GMT
  host: api.spike.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spike Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spike.sh, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Spike.sh
provider_slug: spike-sh
slug: spike-sh-domain-security
source_filename: spike-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spike.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:15:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.spike.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:08:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spike.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:51:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spike.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spike-sh/refs/heads/main/security/spike-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Incident Management
- On-Call
- Alerting
- Escalation Policies
- Status Pages
- Monitoring
- DevOps
- SRE
---
