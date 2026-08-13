---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: discgenics.com
  spf: true
hosts:
- cert_expires: Oct 22 07:38:01 2026 GMT
  host: www.discgenics.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Discgenics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DiscGenics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DiscGenics
provider_slug: discgenics
slug: discgenics-domain-security
source_filename: discgenics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.discgenics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 07:38:01 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: discgenics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discgenics/refs/heads/main/security/discgenics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Biopharmaceutical
- Regenerative Medicine
- Cell Therapy
- Healthcare
- Life Sciences
- Clinical Trials
- Spine
- Utah
---
