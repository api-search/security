---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aiflow.solutions
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: veratainsight.com
  spf: true
hosts:
- cert_expires: Nov 22 18:33:49 2026 GMT
  host: aiflow.solutions
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:28:57 2026 GMT
  host: www.veratainsight.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aiflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aiFlow, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aiFlow
provider_slug: aiflow
slug: aiflow-domain-security
source_filename: aiflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiflow.solutions\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 18:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.veratainsight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:28:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aiflow.solutions\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: veratainsight.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiflow/refs/heads/main/security/aiflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Executive Search
- Private Equity
- Talent Intelligence
- People Data
- Company Data
- Market Intelligence
- Artificial Intelligence
- Y Combinator
- No Public API
---
