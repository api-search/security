---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aiwo.com
  spf: true
hosts:
- cert_expires: Oct 27 11:34:35 2026 GMT
  host: aiwo.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiwo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aiwo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aiwo
provider_slug: aiwo
slug: aiwo-domain-security
source_filename: aiwo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiwo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 11:34:35 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: aiwo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aiwo/refs/heads/main/security/aiwo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Longevity
- Wellness
- Diagnostics
- Artificial Intelligence
---
