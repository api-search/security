---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: future-perfect.co
  spf: true
hosts:
- cert_expires: Nov 11 19:31:59 2026 GMT
  host: www.healthcare.future-perfect.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Future Perfect Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Future Perfect (Healthcare), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Future Perfect (Healthcare)
provider_slug: future-perfect-healthcare
slug: future-perfect-healthcare-domain-security
source_filename: future-perfect-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.healthcare.future-perfect.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 19:31:59 2026 GMT\n  hsts: false\ndomains:\n- domain: future-perfect.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/future-perfect-healthcare/refs/heads/main/security/future-perfect-healthcare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health IT
- Electronic Health Records
- openEHR
- Interoperability
- Clinical Decision Support
- Genomics
- Artificial Intelligence
- NHS
- United Kingdom
---
