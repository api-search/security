---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: truera.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: trulens.org
  spf: false
hosts:
- cert_expires: Sep 14 16:02:17 2026 GMT
  host: truera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 03:58:22 2026 GMT
  host: www.trulens.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TruEra (Snowflake), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TruEra (Snowflake)
provider_slug: truera
slug: truera-domain-security
source_filename: truera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:02:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.trulens.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:58:22 2026 GMT\n  hsts: false\ndomains:\n- domain: truera.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: trulens.org\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truera/refs/heads/main/security/truera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Evaluation
- Observability
- AI Governance
- LLM
- RAG
- Snowflake
---
