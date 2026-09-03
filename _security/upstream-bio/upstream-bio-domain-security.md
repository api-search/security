---
description: ''
domains:
- caa: []
  caa_note: The first probe timed out; a re-query on 2026-09-02 returned cleanly with no CAA record set. Absence of CAA is the finding, not a failed probe.
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upstreambio.com
  nameservers:
  - ns27.domaincontrol.com.
  - ns28.domaincontrol.com.
  spf: true
hosts:
- cert_expires: Nov  8 03:24:42 2026 GMT
  host: upstreambio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upstream Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upstream Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Upstream Bio
provider_slug: upstream-bio
slug: upstream-bio-domain-security
source_filename: upstream-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upstreambio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 03:24:42 2026 GMT\n  hsts: false\ndomains:\n- domain: upstreambio.com\n  dnssec: false\n  caa: []\n  caa_note: >-\n    The first probe timed out; a re-query on 2026-09-02 returned cleanly with no CAA record set.\n    Absence of CAA is the finding, not a failed probe.\n  nameservers:\n  - ns27.domaincontrol.com.\n  - ns28.domaincontrol.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upstream-bio/refs/heads/main/security/upstream-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Healthcare
- Immunology
- Respiratory
- Clinical Trials
- Drug Development
- Nasdaq
---
