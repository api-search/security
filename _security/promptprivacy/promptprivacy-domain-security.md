---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: promptprivacy.com
  spf: true
hosts:
- cert_expires: Dec  2 00:40:57 2026 GMT
  host: promptprivacy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptprivacy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prompt Privacy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Prompt Privacy
provider_slug: promptprivacy
slug: promptprivacy-domain-security
source_filename: promptprivacy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptprivacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 00:40:57 2026 GMT\n  hsts: false\ndomains:\n- domain: promptprivacy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/promptprivacy/security/promptprivacy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Privacy
- Data Governance
- Compliance
---
