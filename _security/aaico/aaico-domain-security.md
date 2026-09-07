---
api_specs:
- filename: postman-collection
  format: yaml
  label: Opus Platform API
  slug: opus-platform-api
  spec_type: Postman
  url: https://developer.opus.com/api-reference/v0-jobs/postman-collection
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aaico.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opus.com
  spf: true
hosts:
- cert_expires: Oct 27 05:28:01 2026 GMT
  host: www.aaico.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 05:31:39 2026 GMT
  host: developer.opus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 00:25:47 2026 GMT
  host: operator.opus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aaico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppliedAI (AAICO), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AppliedAI (AAICO)
provider_slug: aaico
slug: aaico-domain-security
source_filename: aaico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aaico.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 05:28:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.opus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 05:31:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: operator.opus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 00:25:47 2026 GMT\n  hsts: false\ndomains:\n- domain: aaico.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: opus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaico/refs/heads/main/security/aaico-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Workflow Automation
- Agents
- Enterprise
- Document Processing
- Regulated Industries
- Business Process Automation
- Banking
- Insurance
- Healthcare
- Model Context Protocol
---
