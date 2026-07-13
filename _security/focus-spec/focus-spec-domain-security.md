---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: finops.org
  spf: true
hosts:
- cert_expires: Aug 29 00:23:39 2026 GMT
  host: focus.finops.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Focus Spec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FOCUS (FinOps Open Cost and Usage Specification), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FOCUS (FinOps Open Cost and Usage Specification)
provider_slug: focus-spec
slug: focus-spec-domain-security
source_filename: focus-spec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: focus.finops.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:23:39 2026 GMT\n  hsts: false\ndomains:\n- domain: finops.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/focus-spec/refs/heads/main/security/focus-spec-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Billing
- Cost and Usage
- FinOps
- Open Standard
- Specification
---
