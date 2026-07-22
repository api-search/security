---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hyperfinemri.com
  spf: true
hosts:
- cert_expires: Oct  8 15:24:19 2026 GMT
  host: www.hyperfinemri.com
  hsts: true
  hsts_max_age: 31539000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperfine Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyperfine Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hyperfine Research
provider_slug: hyperfine-research
slug: hyperfine-research-domain-security
source_filename: hyperfine-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperfinemri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:24:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31539000\ndomains:\n- domain: hyperfinemri.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperfine-research/refs/heads/main/security/hyperfine-research-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Medical Imaging
- MRI
- Medical Devices
- Healthcare
- Artificial Intelligence
- Neurology
- Point of Care
---
